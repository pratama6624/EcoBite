EcoBite
│
├── App
│   │
│   ├── EcoBiteApp.swift
│   ├── AppDelegate.swift
│   ├── SceneDelegate.swift
│   │
│   ├── AppRouter.swift
│   ├── AppCoordinator.swift
│   ├── AppState.swift
│   ├── AppEnvironment.swift
│   ├── DependencyContainer.swift
│   └── LaunchManager.swift
│
├── Core
│   │
│   ├── Constants
│   │   ├── AppConstant.swift
│   │   ├── ColorConstant.swift
│   │   ├── FontConstant.swift
│   │   ├── AnimationConstant.swift
│   │   ├── APIConstant.swift
│   │   ├── OCRConstant.swift
│   │   └── RiskConstant.swift
│   │
│   ├── Extensions
│   │   ├── String+Extension.swift
│   │   ├── Array+Extension.swift
│   │   ├── Color+Extension.swift
│   │   ├── Date+Extension.swift
│   │   ├── View+Extension.swift
│   │   ├── UIImage+Extension.swift
│   │   └── Bundle+Extension.swift
│   │
│   ├── Helpers
│   │   ├── DateHelper.swift
│   │   ├── NumberFormatterHelper.swift
│   │   ├── ImageHelper.swift
│   │   ├── HapticHelper.swift
│   │   ├── PermissionHelper.swift
│   │   └── FileHelper.swift
│   │
│   ├── Utilities
│   │   ├── Logger.swift
│   │   ├── Validator.swift
│   │   ├── JSONLoader.swift
│   │   ├── ImageCache.swift
│   │   ├── NetworkMonitor.swift
│   │   ├── DeviceInformation.swift
│   │   └── Environment.swift
│   │
│   ├── Protocols
│   │   ├── Repository.swift
│   │   ├── AIProvider.swift
│   │   ├── OCRProvider.swift
│   │   ├── StorageProvider.swift
│   │   └── RiskAnalyzer.swift
│   │
│   ├── Errors
│   │   ├── OCRException.swift
│   │   ├── AIException.swift
│   │   ├── StorageException.swift
│   │   └── ScannerException.swift
│   │
│   └── Managers
│       ├── ThemeManager.swift
│       ├── PermissionManager.swift
│       ├── CameraManager.swift
│       ├── LocationManager.swift
│       └── SessionManager.swift
│
├── Domain
│   │
│   ├── Models
│   │   ├── User.swift
│   │   ├── Questionnaire.swift
│   │   ├── RestrictionProfile.swift
│   │   ├── Ingredient.swift
│   │   ├── IngredientAlias.swift
│   │   ├── IngredientRisk.swift
│   │   ├── ScanResult.swift
│   │   ├── NutritionSummary.swift
│   │   ├── DailyBudget.swift
│   │   ├── ScanHistory.swift
│   │   ├── Product.swift
│   │   └── UserPreference.swift
│   │
│   ├── Enums
│   │   ├── RiskLevel.swift
│   │   ├── IngredientCategory.swift
│   │   ├── DiseaseType.swift
│   │   ├── AllergyType.swift
│   │   ├── DietType.swift
│   │   ├── Gender.swift
│   │   ├── Theme.swift
│   │   └── ScanState.swift
│   │
│   ├── DTO
│   │
│   └── UseCases
│       ├── GenerateProfileUseCase.swift
│       ├── ScanIngredientUseCase.swift
│       ├── AnalyzeRiskUseCase.swift
│       ├── SaveHistoryUseCase.swift
│       ├── LoadHistoryUseCase.swift
│       └── UpdateDailyBudgetUseCase.swift
│
├── Data
│   │
│   ├── Repository
│   │   ├── UserRepository.swift
│   │   ├── QuestionnaireRepository.swift
│   │   ├── IngredientRepository.swift
│   │   ├── RestrictionRepository.swift
│   │   ├── HistoryRepository.swift
│   │   └── NutritionRepository.swift
│   │
│   ├── CoreData
│   │   ├── PersistenceController.swift
│   │   ├── CoreDataStack.swift
│   │   ├── UserEntity.swift
│   │   ├── RestrictionEntity.swift
│   │   ├── IngredientEntity.swift
│   │   ├── HistoryEntity.swift
│   │   └── BudgetEntity.swift
│   │
│   ├── LocalDatabase
│   │   ├── IngredientKnowledge.json
│   │   ├── NutritionDatabase.json
│   │   ├── DiseaseDatabase.json
│   │   └── AliasDatabase.json
│   │
│   └── Cache
│       ├── MemoryCache.swift
│       └── ImageCache.swift
│
├── Services
│   │
│   ├── AI
│   │   ├── AIService.swift
│   │   ├── PromptBuilder.swift
│   │   ├── AIProfileGenerator.swift
│   │   └── AIResponseParser.swift
│   │
│   ├── OCR
│   │   ├── VisionOCRService.swift
│   │   ├── TextRecognizer.swift
│   │   ├── ImagePreprocessor.swift
│   │   └── OCRPostProcessor.swift
│   │
│   ├── Parser
│   │   ├── IngredientParser.swift
│   │   ├── IngredientNormalizer.swift
│   │   ├── IngredientAliasResolver.swift
│   │   └── IngredientMatcher.swift
│   │
│   ├── Analyzer
│   │   ├── RiskAnalyzer.swift
│   │   ├── NutritionAnalyzer.swift
│   │   ├── RestrictionAnalyzer.swift
│   │   └── DailyBudgetAnalyzer.swift
│   │
│   └── Export
│       ├── PDFExporter.swift
│       └── CSVExporter.swift
│
├── Features
│   │
│   ├── Splash
│   ├── Welcome
│   ├── Onboarding
│   ├── Questionnaire
│   ├── AIProfile
│   ├── Home
│   ├── Scanner
│   ├── ScanResult
│   ├── IngredientDetail
│   ├── History
│   ├── DailyBudget
│   ├── Profile
│   ├── Settings
│   └── About
│
│   (Setiap feature memiliki struktur yang sama)
│
│   Scanner
│   │
│   ├── Views
│   │   ├── ScannerView.swift
│   │   ├── CameraView.swift
│   │   ├── ScannerOverlay.swift
│   │   ├── LoadingView.swift
│   │   └── ScannerToolbar.swift
│   │
│   ├── ViewModels
│   │   └── ScannerViewModel.swift
│   │
│   ├── Models
│   │   └── ScannerUIState.swift
│   │
│   ├── Components
│   │   ├── CameraButton.swift
│   │   ├── FocusView.swift
│   │   ├── OCRAnimation.swift
│   │   └── RiskBadge.swift
│   │
│   ├── Coordinator
│   │   └── ScannerCoordinator.swift
│   │
│   └── Preview
│       └── ScannerPreview.swift
│
├── Shared
│   │
│   ├── Components
│   │   ├── PrimaryButton.swift
│   │   ├── SecondaryButton.swift
│   │   ├── LoadingIndicator.swift
│   │   ├── EmptyStateView.swift
│   │   ├── SearchBar.swift
│   │   ├── RiskCard.swift
│   │   ├── IngredientCard.swift
│   │   ├── SectionHeader.swift
│   │   └── CustomNavigationBar.swift
│   │
│   ├── Modifiers
│   │
│   ├── Theme
│   │
│   ├── Styles
│   │
│   └── Animation
│
├── Resources
│   │
│   ├── Assets.xcassets
│   ├── Fonts
│   ├── Localization
│   ├── PreviewContent
│   └── Config
│
└── SupportingFiles
    │
    ├── Info.plist
    ├── EcoBite.entitlements
    └── PrivacyInfo.xcprivacy
