# Softic Solution

## مشروع يحتوي على عدة طبقات بنية (Layered Architecture) وهي:

### 1. **Softic (Presentation Layer - Web API)**

- **Configurations/**: إعدادات الخدمات والميدل وير.
- **Controllers/**: جميع وحدات التحكم في API (مجموعة حسب الميزة).
  - `AuthController.cs`
  - `User/`, `EmployeeControllers/`, `VendorController.cs`, ...
  - ...(30+ مجلد ميزة)
- **Helper/**: المساعدات والخدمات المشتركة.
- **Jobs/**: المهام الخلفية باستخدام Hangfire.
- **Resources/**: ملفات التوطين (Localization) مثل ملفات `.resx`.
- `Program.cs`
- `appsettings.json` و `appsettings.Development.json`
- `Softic.csproj`

### 2. **Softic.BLL (Business Logic Layer)**

- **AuthServices/**: خدمات المصادقة (بما في ذلك تسجيل الدخول عبر Google/Facebook).
- **Enums/**: جميع الثوابت (Enums) للمشروع.
- **Extensions/**: طرق التوسيع (Extension Methods).
- **Helper/**: ردود API، JWT، التصفح (Pagination)...
- **Implementation/**: جميع منطق العمل (Business Logic classes).
  - `UserBL.cs`, `EmployeeBL.cs`, `RequestBL.cs`, ...
  - `UnitOfWork.cs`
- **Interface/**: جميع الواجهات (مثل `IUserBL`, `IEmployeeBL`...).
- **Resolver/**: محولات القيم المخصصة (AutoMapper).
- **Services/**: خدمات خارجية (مثل SMS، FCM، التعرف على الوجه).
- `Softic.BLL.csproj`

### 3. **Softic.DAL (Data Access Layer - Entity Framework)**

- **Database/**:
  - `ApplicationDbContext.cs`
  - `EntityConfigurations/`
- **Entities/**: الكيانات الخاصة بـ EF Core (منظمة حسب الميزة).
  - `Users/`, `EmployeeModels/`, `Requests/`, `Transactions/`, ...
- **Enums/**: ثوابت المشروع.
- **Extends/**: `BaseEntity`, `AppUser`, `IMustHaveCompany`...
- **Migrations/**: الترحيلات بين الإصدارات (مثل 2024 → 2025).
- **Security/**: ملفات الأمان.
- `Softic.DAL.csproj`

### 4. **Softic.DTO (Data Transfer Objects)**

- **AssetsDtos/**, `AuthDtos/`, `EmployeeDtos/`, `RequestDtos/`, ...
- `BaseDto.cs`, `BaseEditDto.cs`
- جميع DTOs الخاصة بالميزات (مثل `Add`, `Edit*`, `Return*`).
- **Lookup/**: جميع DTOs الخاصة بالقيم المرجعية (مثل الفرع، القسم، إلخ).
- `Softic.DTO.csproj`

### 5. **الملفات الأخرى:**
- `Softic.sln`: الملف الرئيسي للحل.
- (مشاريع فرعية أخرى مثل `Softicy.BLL` إذا كان موجودًا).

---

## كيفية العمل مع المشروع

1. **إعداد البيئة**:
   - تأكد من تثبيت الأدوات اللازمة مثل .NET Core.
   - استخدم `dotnet restore` لاستعادة الحزم.

2. **تشغيل التطبيق**:
   - استخدم `dotnet run` لتشغيل API.

3. **إجراء الترحيلات**:
   - استخدم `dotnet ef migrations` لإجراء الترحيلات على قاعدة البيانات.

---

**ملاحظة:** المشروع يستخدم **Hangfire** لتنفيذ المهام في الخلفية، بالإضافة إلى خدمات خارجية مثل **SMS** و **Face Recognition**.

---

### ملاحظة للمطورين الجدد:
يتم تنظيم كل ميزة (feature) في مجلداتها الخاصة داخل الـ **Controllers** و **BLL** و **DAL**، مما يسهل التوسع وإضافة ميزات جديدة.

---

**إعدادات إضافية:**
- `appsettings.json` يحتوي على الإعدادات الرئيسية.
- `appsettings.Development.json` يحتوي على الإعدادات الخاصة ببيئة التطوير.

