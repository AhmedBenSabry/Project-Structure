.
|-- Softic
|   |-- APIGlobale.cs
|   |-- Configurations
|   |   |-- AuthenticationConfg.cs
|   |   |-- ConfigureAppSettings.cs
|   |   |-- DatabaseConfg.cs
|   |   |-- DateOnlySchemaFilter.cs
|   |   |-- ExceptionHandlerConfg.cs
|   |   |-- HangfireConfig.cs
|   |   |-- LocalizationConfig.cs
|   |   `-- ServicesConfg.cs
|   |-- Controllers
|   |   |-- AdminStatics
|   |   |-- Assets
|   |   |-- AuthController.cs
|   |   |-- CommonControllers
|   |   |-- CompanyOffDay
|   |   |-- DashBorad
|   |   |-- EmployeeControllers
|   |   |-- HelpsController
|   |   |-- Issue
|   |   |-- Lookup
|   |   |-- MessageController.cs
|   |   |-- Notification
|   |   |-- Paths
|   |   |-- Payable
|   |   |-- PaymentType
|   |   |-- Receivable
|   |   |-- Request
|   |   |-- RequestReciver
|   |   |-- SuperAdminControllers
|   |   |-- Supports
|   |   |-- Task
|   |   |-- Transactions
|   |   |-- User
|   |   `-- VendorController.cs
|   |-- Helper
|   |   |-- AttendanceReportService.cs
|   |   |-- ConvertBase64ToIFormFile.cs
|   |   |-- EmployeeService.cs
|   |   |-- ExcelImageExtractor.cs
|   |   |-- IAttendanceReportServicecs.cs
|   |   |-- IExcelSheetService.cs
|   |   `-- MapRowToDto.cs
|   |-- Jobs
|   |   `-- MyJob.cs
|   |-- Program.cs
|   |-- Properties
|   |   `-- launchSettings.json
|   |-- Resources
|   |   |-- SharedResources.ar-SA.resx
|   |   |-- SharedResources.cs
|   |   |-- SharedResources.en-US.resx
|   |   `-- SharedResources.resx
|   |-- Softic.csproj
|   |-- Softic.csproj.user
|   |-- appsettings.Development.json
|   |-- appsettings.json
|   `-- notifyfcm-897f3-firebase-adminsdk-ujejf-48e5875f35.json
|-- Softic.BLL
|   |-- AuthServices
|   |   |-- AuthService.cs
|   |   |-- FacebookAuthService.cs
|   |   |-- GoogleAuthService.cs
|   |   |-- IAuthService.cs
|   |   |-- IFacebookAuthService.cs
|   |   `-- IGoogleAuthService.cs
|   |-- BLLGlobale.cs
|   |-- Enums
|   |   |-- ErrorModels.cs
|   |   |-- IssueStatusEnum.cs
|   |   |-- LoginProvider.cs
|   |   |-- NotificationEnum.cs
|   |   `-- RequestCategoryEnum.cs
|   |-- Extensions
|   |   |-- CreateUserFromSocialLoginExtension.cs
|   |   `-- GeoUtils.cs
|   |-- Helper
|   |   |-- ApiResponse.cs
|   |   |-- BroadnetSettings.cs
|   |   |-- DomainProfile.cs
|   |   |-- EntitySC.cs
|   |   |-- FacebookAuthSettings.cs
|   |   |-- FacebookTokenValidationResponse.cs
|   |   |-- FacebookUserInfoResponse.cs
|   |   |-- GoogleAuthSettings.cs
|   |   |-- JWT.cs
|   |   |-- Pagination.cs
|   |   |-- UnifonicSettings.cs
|   |   `-- WasageSettings.cs
|   |-- Implementation
|   |   |-- Assets
|   |   |-- BaseRepo.cs
|   |   |-- CompanyBL.cs
|   |   |-- CompanyOffDayBL.cs
|   |   |-- CompanySubscriptionBL.cs
|   |   |-- DashboardBL
|   |   |-- EmployeeBL
|   |   |-- HelpsBL
|   |   |-- Issue
|   |   |-- Lookup
|   |   |-- NotificationBL
|   |   |-- PathsBL
|   |   |-- PaymentTypeBL
|   |   |-- RequestApprovalMatrix
|   |   |-- RequestBL
|   |   |-- SendMessage
|   |   |-- SubscriptionPlanBL.cs
|   |   |-- SupportsBL
|   |   |-- TasksBL
|   |   |-- TransactionBL
|   |   |-- UnitOfWork.cs
|   |   |-- UserBL
|   |   |-- VendorBL
|   |   `-- VendorTypeBL
|   |-- Interface
|   |   |-- Assets
|   |   |-- IBaseRepo.cs
|   |   |-- ICompanyBL.cs
|   |   |-- ICompanyOffDayBL
|   |   |-- ICompanySubscriptionBL.cs
|   |   |-- IDashboardBL
|   |   |-- IEmployeeBL
|   |   |-- IHelpsBL
|   |   |-- IIssue
|   |   |-- INotificationBL
|   |   |-- IPathsBL
|   |   |-- IPaymentTypeBL
|   |   |-- IRequestBL
|   |   |-- ISendMessage
|   |   |-- ISubscriptionPlanBL.cs
|   |   |-- ISupportsBL
|   |   |-- ITasksBL
|   |   |-- ITransactionBL
|   |   |-- IUnitOfWork.cs
|   |   |-- IUserBL
|   |   |-- IVendorBL
|   |   |-- IVendorTypeBL.cs
|   |   |-- Lookup
|   |   `-- RequestApprovalMatrix
|   |-- Resolver
|   |   |-- Asset
|   |   |-- AttendanceEmployeeProfileImageResolver.cs
|   |   |-- AttendancePhotoResolver.cs
|   |   |-- AttendanceSignatureResolver.cs
|   |   |-- BankTransfareFromEmployeeResolver.cs
|   |   |-- CompanyImgResolver.cs
|   |   |-- EmployeeCertificateFileResolver.cs
|   |   |-- EmployeeEducationalFileResolver.cs
|   |   |-- EmployeeIdentityDocumentFileResolver.cs
|   |   |-- EmployeeNameResolver.cs
|   |   |-- EmployeeNationalIdPhotoImgResolver.cs
|   |   |-- EmployeePassportPhotoImgResolver.cs
|   |   |-- EmployeeReferancePhotoImgResolver.cs
|   |   |-- EmployeeWorkHistoryFileResolver.cs
|   |   |-- HelpAttachmentFileResolver.cs
|   |   |-- IssueAttachmentFileResolver.cs
|   |   |-- OnBoardingImgResolver.cs
|   |   |-- PayableTransactionAttachmentResolver.cs
|   |   |-- ProfileImageImgResolver.cs
|   |   |-- ReferancePhotoImgResolver.cs
|   |   |-- Request
|   |   |-- RequestTypeImgResolver.cs
|   |   |-- ReturnToDoItemProfileImageResolver.cs
|   |   |-- SupportAttachmentFileResolver.cs
|   |   |-- TaskAttachmentFileResolver.cs
|   |   |-- TransactionAttachmentResolver.cs
|   |   |-- UserAttachmentImgResolver.cs
|   |   `-- UserProfileImageResolver.cs
|   |-- Services
|   |   |-- FaceRecognationServices
|   |   |-- FileServices
|   |   |-- NotificationServices
|   |   `-- Sms
|   `-- Softic.BLL.csproj
|-- Softic.DAL
|   |-- DALGlobal.cs
|   |-- Database
|   |   |-- ApplicationDbContext.cs
|   |   `-- EntityConfigurations
|   |-- Entities
|   |   |-- Asset
|   |   |-- Company.cs
|   |   |-- CompanyOffDay.cs
|   |   |-- CompanySubscription.cs
|   |   |-- EmployeeModels
|   |   |-- Helps
|   |   |-- Lookup
|   |   |-- Notification
|   |   |-- OrganizationChart.cs
|   |   |-- Paths
|   |   |-- RequestApprovalMatrix
|   |   |-- Requests
|   |   |-- SubscriptionPlan.cs
|   |   |-- Suggestions&Complains
|   |   |-- Supports
|   |   |-- Tasks
|   |   |-- Transactions
|   |   |-- Users
|   |   |-- Vendor
|   |   `-- VendorType
|   |-- Enums
|   |   |-- AccountStatusEnum.cs
|   |   |-- AssetSatausEnum.cs
|   |   |-- AttendanceTypeEnum.cs
|   |   |-- BankTransfareStatus.cs
|   |   |-- Gender.cs
|   |   |-- ReceivableStatus.cs
|   |   |-- RequestStatusEnum.cs
|   |   `-- UserTypeEnum.cs
|   |-- Extends
|   |   |-- AppUser.cs
|   |   |-- BaseEntity.cs
|   |   |-- EmailDetails.cs
|   |   |-- HealthInformation.cs
|   |   |-- IMustHaveCompany.cs
|   |   `-- TelephoneDetails.cs
|   |-- Migrations
|   |   |-- 20250128092111_Inital.Designer.cs
|   |   |-- 20250128092111_Inital.cs
|   |   |-- 20250129090054_HandleOrgChart.Designer.cs
|   |   |-- 20250129090054_HandleOrgChart.cs
|   |   |-- 20250129193151_DueDate_Tasks.Designer.cs
|   |   |-- 20250129193151_DueDate_Tasks.cs
|   |   |-- 20250130104102_EditTodoList.Designer.cs
|   |   |-- 20250130104102_EditTodoList.cs
|   |   |-- 20250204111401_AddBranchToTask.Designer.cs
|   |   |-- 20250204111401_AddBranchToTask.cs
|   |   |-- 20250206102812_Team.Designer.cs
|   |   |-- 20250206102812_Team.cs
|   |   |-- 20250206111347_ExpiryDate.Designer.cs
|   |   |-- 20250206111347_ExpiryDate.cs
|   |   |-- 20250206112727_AddteamToTask.Designer.cs
|   |   |-- 20250206112727_AddteamToTask.cs
|   |   |-- 20250210101206_Support_CompanyField.Designer.cs
|   |   |-- 20250210101206_Support_CompanyField.cs
|   |   |-- 20250212132437_VacationToHr.Designer.cs
|   |   |-- 20250212132437_VacationToHr.cs
|   |   |-- 20250226095845_EditIssueTitle.Designer.cs
|   |   |-- 20250226095845_EditIssueTitle.cs
|   |   |-- 20250226101312_CompanyColor_Removing.Designer.cs
|   |   |-- 20250226101312_CompanyColor_Removing.cs
|   |   |-- 20250227045215_HelpModule.Designer.cs
|   |   |-- 20250227045215_HelpModule.cs
|   |   |-- 20250319131333_EditSeedIssueStatus.Designer.cs
|   |   |-- 20250319131333_EditSeedIssueStatus.cs
|   |   |-- 20250406132429_GHJH.Designer.cs
|   |   |-- 20250406132429_GHJH.cs
|   |   |-- 20250408130225_AddCompanySubscriptionsTable.Designer.cs
|   |   |-- 20250408130225_AddCompanySubscriptionsTable.cs
|   |   |-- 20250409110720_AddStartShiftTimeTableCompanyAndAddIsDelay,DelayTimeTableEmployeeAttendance.Designer.cs
|   |   |-- 20250409110720_AddStartShiftTimeTableCompanyAndAddIsDelay,DelayTimeTableEmployeeAttendance.cs
|   |   |-- 20250409112244_RemoveIsDalayAndDelayTimeFromEmployeeAttendance.Designer.cs
|   |   |-- 20250409112244_RemoveIsDalayAndDelayTimeFromEmployeeAttendance.cs
|   |   |-- 20250409131241_Add MeetingDate Table CompanySubscription.Designer.cs
|   |   |-- 20250409131241_Add MeetingDate Table CompanySubscription.cs
|   |   |-- 20250413121824_Add Message, IsMessage, IsMeeting, and SubscriptionPlan to CompanySubscription.Designer.cs
|   |   |-- 20250413121824_Add Message, IsMessage, IsMeeting, and SubscriptionPlan to CompanySubscription.cs
|   |   |-- 20250413132739_Remove IsMessage,and IsMeeting From CompanySubscription.Designer.cs
|   |   |-- 20250413132739_Remove IsMessage,and IsMeeting From CompanySubscription.cs
|   |   |-- 20250414091718_HandleDateDay.Designer.cs
|   |   |-- 20250414091718_HandleDateDay.cs
|   |   |-- 20250420120513_RemoveWeekEndes.Designer.cs
|   |   |-- 20250420120513_RemoveWeekEndes.cs
|   |   |-- 20250422113114_Add EmployeeAttendance To Employee.Designer.cs
|   |   |-- 20250422113114_Add EmployeeAttendance To Employee.cs
|   |   |-- 20250422152619_Edittttttttttt.Designer.cs
|   |   |-- 20250422152619_Edittttttttttt.cs
|   |   |-- 20250504130330_EditLongAndLat.Designer.cs
|   |   |-- 20250504130330_EditLongAndLat.cs
|   |   |-- 20250504133436_EditLongAndLatsfwe.Designer.cs
|   |   |-- 20250504133436_EditLongAndLatsfwe.cs
|   |   |-- 20250507094645_EDitfgmvsd.Designer.cs
|   |   |-- 20250507094645_EDitfgmvsd.cs
|   |   |-- 20250507130118_Edit BusinessSize Data.Designer.cs
|   |   |-- 20250507130118_Edit BusinessSize Data.cs
|   |   |-- 20250526123925_AddCommentPropertyToTableRequest.Designer.cs
|   |   |-- 20250526123925_AddCommentPropertyToTableRequest.cs
|   |   |-- 20250528090113_HUIKJN.Designer.cs
|   |   |-- 20250528090113_HUIKJN.cs
|   |   |-- 20250528091315_HUIKJNDASSAd.Designer.cs
|   |   |-- 20250528091315_HUIKJNDASSAd.cs
|   |   |-- 20250528092743_HUIKJNDASSAdjkn.Designer.cs
|   |   |-- 20250528092743_HUIKJNDASSAdjkn.cs
|   |   |-- 20250528102152_HUIKJNDASSAdjknjihuij.Designer.cs
|   |   |-- 20250528102152_HUIKJNDASSAdjknjihuij.cs
|   |   |-- 20250622084557_EmployeeCode.Designer.cs
|   |   |-- 20250622084557_EmployeeCode.cs
|   |   |-- 20250626130717_DeleteAcc.Designer.cs
|   |   |-- 20250626130717_DeleteAcc.cs
|   |   |-- 20250706085921_AddCompanySizeAndCompanyModule.Designer.cs
|   |   |-- 20250706085921_AddCompanySizeAndCompanyModule.cs
|   |   |-- 20250708102812_Add Branch To EmployeeAttendanceLocation.Designer.cs
|   |   |-- 20250708102812_Add Branch To EmployeeAttendanceLocation.cs
|   |   |-- 20250714100559_Add ReferancePhoto And Signature To Company.Designer.cs
|   |   |-- 20250714100559_Add ReferancePhoto And Signature To Company.cs
|   |   |-- 20250714120654_Remove Flags From Company.Designer.cs
|   |   |-- 20250714120654_Remove Flags From Company.cs
|   |   |-- 20250715075119_Add Company ReferancePhotoFlag And SignatureFlag.Designer.cs
|   |   |-- 20250715075119_Add Company ReferancePhotoFlag And SignatureFlag.cs
|   |   |-- 20250716090454_Change properties To ReferancePhotoIsRequired And SignatureIsRequired.Designer.cs
|   |   |-- 20250716090454_Change properties To ReferancePhotoIsRequired And SignatureIsRequired.cs
|   |   |-- 20250716115936_Make Photo, Signature Properties Nullable Taple EmployeeAttendance.Designer.cs
|   |   |-- 20250716115936_Make Photo, Signature Properties Nullable Taple EmployeeAttendance.cs
|   |   |-- 20250729102813_AttendanceMain.Designer.cs
|   |   |-- 20250729102813_AttendanceMain.cs
|   |   |-- 20250729103706_AttendanceMainEdit.Designer.cs
|   |   |-- 20250729103706_AttendanceMainEdit.cs
|   |   |-- 20250825102941_Add CompanyModules.Designer.cs
|   |   |-- 20250825102941_Add CompanyModules.cs
|   |   |-- 20250825122255_Add OffDays To Company.Designer.cs
|   |   |-- 20250825122255_Add OffDays To Company.cs
|   |   |-- 20250825135419_Add Daysoff To Company.Designer.cs
|   |   |-- 20250825135419_Add Daysoff To Company.cs
|   |   |-- 20250825142006_Add Percentage To BenefitType.Designer.cs
|   |   |-- 20250825142006_Add Percentage To BenefitType.cs
|   |   |-- 20250827110037_EmployeeSalaryWithAllow.Designer.cs
|   |   |-- 20250827110037_EmployeeSalaryWithAllow.cs
|   |   |-- 20250828084141_Add DaysFromHome.Designer.cs
|   |   |-- 20250828084141_Add DaysFromHome.cs
|   |   |-- 20250901113450_AddRequestAttachmentTitle.Designer.cs
|   |   |-- 20250901113450_AddRequestAttachmentTitle.cs
|   |   |-- 20250901150547_AddRequestFileName.Designer.cs
|   |   |-- 20250901150547_AddRequestFileName.cs
|   |   |-- 20250902080324_EmployeeAttendanceMainEdit.Designer.cs
|   |   |-- 20250902080324_EmployeeAttendanceMainEdit.cs
|   |   |-- 20250902080913_EmployeeAttendanceMainEditABS.Designer.cs
|   |   |-- 20250902080913_EmployeeAttendanceMainEditABS.cs
|   |   |-- 20250902082847_EmployeeAttendanceMainEditABSNULL.Designer.cs
|   |   |-- 20250902082847_EmployeeAttendanceMainEditABSNULL.cs
|   |   |-- 20250903113832_RemoveFileNameFromRequestAttachment.Designer.cs
|   |   |-- 20250903113832_RemoveFileNameFromRequestAttachment.cs
|   |   |-- 20250907132357_Add Paths and Points.Designer.cs
|   |   |-- 20250907132357_Add Paths and Points.cs
|   |   |-- 20250907141334_CompanyOffDay.Designer.cs
|   |   |-- 20250907141334_CompanyOffDay.cs
|   |   |-- 20250907211942_CompanyOffDayTestEnv.Designer.cs
|   |   |-- 20250907211942_CompanyOffDayTestEnv.cs
|   |   |-- 20250908074412_Add EmployeePath.Designer.cs
|   |   |-- 20250908074412_Add EmployeePath.cs
|   |   |-- 20250908092951_Add Table EmployeePath.Designer.cs
|   |   |-- 20250908092951_Add Table EmployeePath.cs
|   |   |-- 20250908113419_AddVendorsAndVendorTypes.Designer.cs
|   |   |-- 20250908113419_AddVendorsAndVendorTypes.cs
|   |   |-- 20250909122445_Add Customer.Designer.cs
|   |   |-- 20250909122445_Add Customer.cs
|   |   |-- 20250909224127_AddPayableAndReciveable.Designer.cs
|   |   |-- 20250909224127_AddPayableAndReciveable.cs
|   |   |-- 20250910092913_AdjustPayableAndReceivable.Designer.cs
|   |   |-- 20250910092913_AdjustPayableAndReceivable.cs
|   |   |-- 20250910120207_DeletePathIdFromCustomer.Designer.cs
|   |   |-- 20250910120207_DeletePathIdFromCustomer.cs
|   |   |-- 20250910120247_Edit Customer.Designer.cs
|   |   |-- 20250910120247_Edit Customer.cs
|   |   |-- 20250910122436_Edit Customer Table.Designer.cs
|   |   |-- 20250910122436_Edit Customer Table.cs
|   |   |-- 20250910124443_EditPathsWithCustomer.Designer.cs
|   |   |-- 20250910124443_EditPathsWithCustomer.cs
|   |   |-- 20250916111534_AddEmployeeSalaryArchive.Designer.cs
|   |   |-- 20250916111534_AddEmployeeSalaryArchive.cs
|   |   |-- 20250916130136_EmployeeSalaryArchiveNullableFullName.Designer.cs
|   |   |-- 20250916130136_EmployeeSalaryArchiveNullableFullName.cs
|   |   |-- 20250923134322_AddPaymentType.Designer.cs
|   |   |-- 20250923134322_AddPaymentType.cs
|   |   |-- 20250928103420_Add CustomerRelatedTo.Designer.cs
|   |   |-- 20250928103420_Add CustomerRelatedTo.cs
|   |   |-- 20250928115825_Add RelatedTo.Designer.cs
|   |   |-- 20250928115825_Add RelatedTo.cs
|   |   |-- 20250930084152_Add FinancialCustodies.Designer.cs
|   |   |-- 20250930084152_Add FinancialCustodies.cs
|   |   |-- 20250930100154_Add FinancialCustodiesDbset.Designer.cs
|   |   |-- 20250930100154_Add FinancialCustodiesDbset.cs
|   |   |-- 20250930114351_Add Custom Validation On FinancialCustodiesDbset.Designer.cs
|   |   |-- 20250930114351_Add Custom Validation On FinancialCustodiesDbset.cs
|   |   |-- 20251001111026_Add BankTransfareFromEmployee.Designer.cs
|   |   |-- 20251001111026_Add BankTransfareFromEmployee.cs
|   |   |-- 20251002101006_AttachmentPayable.Designer.cs
|   |   |-- 20251002101006_AttachmentPayable.cs
|   |   |-- 20251002121257_RejectReason.Designer.cs
|   |   |-- 20251002121257_RejectReason.cs
|   |   |-- 20251002132324_RejectReasonBank.Designer.cs
|   |   |-- 20251002132324_RejectReasonBank.cs
|   |   |-- 20251007101502_DayOfWdsad.Designer.cs
|   |   |-- 20251007101502_DayOfWdsad.cs
|   |   |-- 20251008134856_RefernceTypeNullable.Designer.cs
|   |   |-- 20251008134856_RefernceTypeNullable.cs
|   |   |-- 20251008142526_BloodTypeNullable.Designer.cs
|   |   |-- 20251008142526_BloodTypeNullable.cs
|   |   |-- 20251012115132_NullableEmployeeWorkHistory.Designer.cs
|   |   |-- 20251012115132_NullableEmployeeWorkHistory.cs
|   |   |-- 20251012120936_MakeSkillTypeNullableInEmployeeSkill.Designer.cs
|   |   |-- 20251012120936_MakeSkillTypeNullableInEmployeeSkill.cs
|   |   |-- 20251012122401_MakeUserAttachmentFieldsOptional.Designer.cs
|   |   |-- 20251012122401_MakeUserAttachmentFieldsOptional.cs
|   |   |-- 20251012122850_MakeUserAttachmentNameOptional.Designer.cs
|   |   |-- 20251012122850_MakeUserAttachmentNameOptional.cs
|   |   |-- 20251015100117_GUJkm.Designer.cs
|   |   |-- 20251015100117_GUJkm.cs
|   |   |-- 20251016110207_DAdas.Designer.cs
|   |   |-- 20251016110207_DAdas.cs
|   |   |-- 20251021114501_FSsdfdsf.Designer.cs
|   |   |-- 20251021114501_FSsdfdsf.cs
|   |   |-- 20251021124640_FSsdfdsfASDAsdwe.Designer.cs
|   |   |-- 20251021124640_FSsdfdsfASDAsdwe.cs
|   |   |-- 20251027100856_DSAd.Designer.cs
|   |   |-- 20251027100856_DSAd.cs
|   |   |-- 20251027111827_Entitlment.Designer.cs
|   |   |-- 20251027111827_Entitlment.cs
|   |   |-- 20251027120358_Deduction.Designer.cs
|   |   |-- 20251027120358_Deduction.cs
|   |   |-- 20251029104823_MassiveActionTransaction.Designer.cs
|   |   |-- 20251029104823_MassiveActionTransaction.cs
|   |   |-- 20251029105150_MassiveActionTransactionasdasd.Designer.cs
|   |   |-- 20251029105150_MassiveActionTransactionasdasd.cs
|   |   |-- 20251029111522_MassiveActionTransactionasdasdfew.Designer.cs
|   |   |-- 20251029111522_MassiveActionTransactionasdasdfew.cs
|   |   |-- 20251029114122_MassiveActionTransactionasdasdfewrferf.Designer.cs
|   |   |-- 20251029114122_MassiveActionTransactionasdasdfewrferf.cs
|   |   |-- 20251102110230_Sfef.Designer.cs
|   |   |-- 20251102110230_Sfef.cs
|   |   |-- 20251104131101_ASDefwd.Designer.cs
|   |   |-- 20251104131101_ASDefwd.cs
|   |   |-- 20251109114453_TEamLocation.Designer.cs
|   |   |-- 20251109114453_TEamLocation.cs
|   |   |-- 20251111145724_IsSmartRequest.Designer.cs
|   |   |-- 20251111145724_IsSmartRequest.cs
|   |   |-- 20251119101731_AA.Designer.cs
|   |   |-- 20251119101731_AA.cs
|   |   `-- ApplicationDbContextModelSnapshot.cs
|   |-- Security
|   |   `-- DecodeAndEncode.cs
|   `-- Softic.DAL.csproj
|-- Softic.DTO
|   |-- AddBaseDtoForExcel.cs
|   |-- AssetsDtos
|   |   |-- AddAssetCategoryDto.cs
|   |   |-- AddAssetCategoryDtoForExcel.cs
|   |   |-- AssetAttachmentDtos
|   |   |-- AssetCategoryCountDto.cs
|   |   |-- AssetCategoryFileDto.cs
|   |   |-- AssetCountPerMonthDto.cs
|   |   |-- AssetCountRequestDto.cs
|   |   |-- AssetCountRequestEmployeeDto.cs
|   |   |-- AssetDtos
|   |   |-- EditAssetCategoryDto.cs
|   |   |-- EmployeeAssetCountRequestDto.cs
|   |   |-- RelatedAssetDtos
|   |   `-- ReturnAssetCategoryDto.cs
|   |-- AuthDtos
|   |   |-- AddAdminDto.cs
|   |   |-- AddUserDtoForExcel.cs
|   |   |-- AuthModel.cs
|   |   |-- CreateUserFromSocialLogin.cs
|   |   |-- EditAccountStatusDto.cs
|   |   |-- FacebookSignInDto.cs
|   |   |-- ForgetPasswordDto.cs
|   |   |-- GoogleSignInDto.cs
|   |   |-- LoginDto.cs
|   |   |-- LoginNFCDto.cs
|   |   |-- RegisterDto.cs
|   |   |-- ResetPasswordDto.cs
|   |   |-- UserDto.cs
|   |   |-- UserFileDto.cs
|   |   `-- VerfiyPhoneNumberDto.cs
|   |-- BankTransfareFromEmployeeDtos
|   |   |-- AddBankTransfareFromEmployeeDto.cs
|   |   |-- ChangeBankTransfareFromEmployeeStatusDto.cs
|   |   |-- EditBankTransfareFromEmployeeDto.cs
|   |   `-- ReturnBankTransfareFromEmployeeDto.cs
|   |-- BaseDto.cs
|   |-- BaseEditDto.cs
|   |-- BaseFileDto.cs
|   |-- CompanyDtos
|   |   |-- AddCompanyDto.cs
|   |   |-- CompanySubscriptionDtos
|   |   |-- EditCompanyDto.cs
|   |   |-- EditCompanySettingDto.cs
|   |   |-- ReturnCompanyDto.cs
|   |   |-- ReturnCompanyEmployeeStaticsDto.cs
|   |   |-- ReturnCompanyEmployeesCheckInAndOutStaticsDto.cs
|   |   |-- SubscriptionPlanDtos
|   |   |-- SupportAttachmentDtos
|   |   `-- SupportDtos
|   |-- CompanyOffDayDtos
|   |   |-- AddCompanyOffDayDto.cs
|   |   |-- EditCompanyOffDayDto.cs
|   |   `-- ReturnCompanyOffDayDto.cs
|   |-- DTOGlobal.cs
|   |-- DashboardDtos
|   |   `-- ReturnDashboardDto.cs
|   |-- EmployeeAttendanceLocationDtos
|   |   |-- AddEmployeeAttendanceLocationDto.cs
|   |   |-- EditEmployeeAttendanceLocationDto.cs
|   |   `-- ReturnEmployeeAttendanceLocationDto.cs
|   |-- EmployeeDtos
|   |   |-- AddEmployeeDto.cs
|   |   |-- AddEmployeeInfoDto.cs
|   |   |-- AddEmployeeLevelSettingAssignment.cs
|   |   |-- AssginEmployeeSalaryDto.cs
|   |   |-- AssginEmployeeShiftDto.cs
|   |   |-- AssignEmployeeHiringDateDto.cs
|   |   |-- AssignEmployeeLevelDto.cs
|   |   |-- Attendance
|   |   |-- EditEmployeeDto.cs
|   |   |-- EducationalDtos
|   |   |-- EmployeeAssginBranchDto.cs
|   |   |-- EmployeeAssginDepartmentDto.cs
|   |   |-- EmployeeAssginPositionDto.cs
|   |   |-- EmployeeCertificateDtos
|   |   |-- EmployeeDeductionDtos
|   |   |-- EmployeeEntitlmentDtos
|   |   |-- EmployeeHealthInformationDtos
|   |   |-- EmployeeIdentityDocumentDtos
|   |   |-- EmployeeLanguageDtos
|   |   |-- EmployeeLevelDtos
|   |   |-- EmployeeLevelSettingsDtos
|   |   |-- EmployeeSalaryArchiveDtos
|   |   |-- EmployeeSkillsDtos
|   |   |-- MassiveActionDto.cs
|   |   |-- MassiveActionTransactionDtos
|   |   |-- ReturnEmployeeDto.cs
|   |   |-- ReturnEmployeeLevelSettingAssignment.cs
|   |   |-- ReturnEmployeeSalariesExportDto.cs
|   |   |-- ReturnEmployeeSalaryReportDto.cs
|   |   |-- SaveEmployeeSalaryDto.cs
|   |   |-- UpdateReferencePhotoDto.cs
|   |   |-- Vacation
|   |   `-- WorkHistoryDtos
|   |-- FaceRecognationDtos
|   |   |-- CheckUserReferancePhoto.cs
|   |   |-- RecognationCheckDto.cs
|   |   `-- RecognationResponseDto.cs
|   |-- FinancialCustodyDtos
|   |   |-- AddFinancialCustodyDto.cs
|   |   |-- EditFinancialCustodyDto.cs
|   |   |-- FinancialCustodyCollect.cs
|   |   `-- ReturnFinancialCustodyDto.cs
|   |-- HelpDtos
|   |   |-- HelpAttachmentDto
|   |   `-- HelpDto
|   |-- IssueDtos
|   |   |-- AddIssueDto.cs
|   |   |-- AgainestTypeDtos
|   |   |-- EditIssueDto.cs
|   |   |-- IssueActionDto.cs
|   |   |-- IssueAttachmentDtos
|   |   |-- IssueCommentDtos
|   |   |-- IssueExcuterDtos
|   |   |-- IssueStatusDtos
|   |   |-- IssueTypeDtos
|   |   `-- ReturnIssueDto.cs
|   |-- Lookup
|   |   |-- AttachmentCategoryDtos
|   |   |-- AttendanceTypeDtos
|   |   |-- BloodTypeDtos
|   |   |-- BranchDtos
|   |   |-- BusinessSizeDtos
|   |   |-- BusinessTypeDtos
|   |   |-- CertificateTypeDtos
|   |   |-- CountryDtos
|   |   |-- CtiyDots
|   |   |-- CurrencyDtos
|   |   |-- DeductionTypeDtos
|   |   |-- DegreeDtos
|   |   |-- DepartmentDtos
|   |   |-- DocumentTypeDtos
|   |   |-- EntitlmentTypeDtos
|   |   |-- FileDescriptionDtos
|   |   |-- FileDescriptionTypeDtos
|   |   |-- GradeDtos
|   |   |-- LanguageDtos
|   |   |-- LifeStyleTypeDtos
|   |   |-- MedicalInsuranceCompanyDtos
|   |   |-- OnBoardingDtos
|   |   |-- OrganizationChart
|   |   |-- PersonalTypeDtos
|   |   |-- PositionDtos
|   |   |-- PositionTypeDtos
|   |   |-- RefernceTypeDtos
|   |   |-- SkillsTypeDtos
|   |   |-- TaskPriorityDtos
|   |   |-- TaskStatusDtos
|   |   |-- TeamDtos
|   |   |-- UniversityDtos
|   |   `-- ZoneDtos
|   |-- NotificationDtos
|   |   `-- NotificationTemp.cs
|   |-- NotificationLogDtos
|   |   |-- AddNotificationLogDto.cs
|   |   |-- EditNotificationLogDto.cs
|   |   `-- ReturnNotificationLogDto.cs
|   |-- PathsDtos
|   |   |-- AddCustomerPathDto.cs
|   |   |-- AddEmployeePathDto.cs
|   |   |-- AddPathsDto.cs
|   |   |-- CustomersDtos
|   |   |-- EditCustomerPathDto.cs
|   |   |-- EditEmployeePathDto.cs
|   |   |-- EditPathsDto.cs
|   |   |-- ReturnCustomerPath.cs
|   |   |-- ReturnEmployeePath.cs
|   |   `-- ReturnPathsDto.cs
|   |-- PayableDtos
|   |   |-- AddPayableDto.cs
|   |   |-- EditPayableDto.cs
|   |   `-- ReturnPayableDto.cs
|   |-- PaymentTypeDto
|   |   |-- AddPaymentTypeDto.cs
|   |   |-- EditPaymentTypeDto.cs
|   |   `-- ReturnPaymentTypeDto.cs
|   |-- ReceivableDtos
|   |   |-- AddReceivableDto.cs
|   |   |-- ChangeReceivableStatusDto.cs
|   |   |-- EditReceivableDto.cs
|   |   `-- ReturnReceivableDto.cs
|   |-- RequestApprovalMatrixDtos
|   |   `-- ReturnRequestApprovalMatrixDto.cs
|   |-- RequestDtos
|   |   |-- AcceptRequestWithReason.cs
|   |   |-- ActionRequestDto.cs
|   |   |-- AddRequestDto.cs
|   |   |-- EditRequestDto.cs
|   |   |-- EmployeeRequestDto.cs
|   |   |-- RequestAttachmentDtos
|   |   |-- RequestCategoryDtos
|   |   |-- RequestStatusDtos
|   |   |-- RequestTypeDtos
|   |   `-- ReturnRequestDto.cs
|   |-- SmsDtos
|   |   `-- FCMMessageDto.cs
|   |-- Softic.DTO.csproj
|   |-- TaskManagementDto
|   |   |-- ArchivedTaskDto
|   |   |-- CostDto
|   |   |-- EvaluationDto
|   |   |-- TaskAssignmentDto
|   |   |-- TaskAttachmentDto
|   |   |-- TasksDto
|   |   `-- ToDoItemDto
|   |-- TransactionsDto
|   |   |-- AddTransactionDto.cs
|   |   |-- EditTransactionDto.cs
|   |   `-- ReturnTransactionDto.cs
|   |-- UserDtos
|   |   |-- AddUserSocailDto.cs
|   |   |-- AddressesDtos
|   |   |-- AttachmentDtos
|   |   |-- EditUserInfoDto.cs
|   |   |-- EmailDtos
|   |   |-- LifeStyleDtos
|   |   |-- RefernceDtos
|   |   |-- ReturnUserDto.cs
|   |   |-- ReturnUserInfoDto.cs
|   |   |-- ReturnUserSocailDto.cs
|   |   `-- TelephoneDto
|   |-- VendorDto
|   |   |-- AddVendorDto.cs
|   |   |-- EditVendorDto.cs
|   |   `-- ReturnVendorDto.cs
|   |-- VendorTypeDto
|   |   |-- AddVendorTypeDto.cs
|   |   |-- EditVendorTypeDto.cs
|   |   `-- ReturnVendorTypeDto.cs
|   `-- Wasage
|       |-- WasageCallBackDto.cs
|       `-- WasageResponseDto.cs
|-- Softic.sln







