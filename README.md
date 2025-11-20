Softic.Solution/
├── Softic (Presentation Layer - Web API)
│   ├── Configurations/              # All services & middleware config
│   ├── Controllers/                 # All API controllers (grouped by feature)
│   │   ├── AuthController.cs
│   │   ├── User/, EmployeeControllers/, VendorController.cs, ...
│   │   └── ... (30+ feature folders)
│   ├── Helper/                      # Shared helpers & services
│   ├── Jobs/                        # Hangfire / Background jobs
│   ├── Resources/                   # Localization (.resx files)
│   ├── Program.cs
│   ├── appsettings.json + appsettings.Development.json
│   └── Softic.csproj
│
├── Softic.BLL (Business Logic Layer)
│   ├── AuthServices/                # Auth + Social login (Google/Facebook)
│   ├── Enums/                       # All project enums
│   ├── Extensions/                  # Extension methods
│   ├── Helper/                      # API responses, JWT, Pagination...
│   ├── Implementation/              # All Business Logic classes (BL.cs)
│   │   ├── UserBL.cs, EmployeeBL.cs, RequestBL.cs, ...
│   │   └── UnitOfWork.cs
│   ├── Interface/                   # All interfaces (IUserBL, IEmployeeBL...)
│   ├── Resolver/                    # Custom value resolvers (AutoMapper)
│   ├── Services/                    # External services (SMS, FCM, Face Recognition)
│   └── Softic.BLL.csproj
│
├── Softic.DAL (Data Access Layer - Entity Framework)
│   ├── Database/
│   │   ├── ApplicationDbContext.cs
│   │   └── EntityConfigurations/
│   ├── Entities/                    # All EF Core entities (organized by feature)
│   │   ├── Users/, EmployeeModels/, Requests/, Transactions/, ...
│   ├── Enums/
│   ├── Extends/                     # BaseEntity, AppUser, IMustHaveCompany...
│   ├── Migrations/                  # 2024 → 2025 migrations (very active project!)
│   ├── Security/
│   └── Softic.DAL.csproj
│
├── Softic.DTO (Data Transfer Objects)
│   ├── AssetsDtos/, AuthDtos/, EmployeeDtos/, RequestDtos/, ...
│   ├── BaseDto.cs, BaseEditDto.cs
│   ├── All feature-specific DTOs (Add, Edit*, Return*)
│   ├── Lookup/                      # All lookup DTOs (Branch, Department, etc.)
│   └── Softic.DTO.csproj
│
└── Softic.sln                       # Main solution file
 
