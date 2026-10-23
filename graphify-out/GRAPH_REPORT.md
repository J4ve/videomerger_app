# Graph Report - videomerger_app  (2026-10-23)

## Corpus Check
- Large corpus: 500 files · ~680,437 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 2297 nodes · 3643 edges · 161 communities (155 shown, 3 thin omitted)
- Extraction: 87% EXTRACTED · 13% INFERRED · 0% AMBIGUOUS · INFERRED: 459 edges (avg confidence: 0.91)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- AdminDashboard
- SessionManager
- .create_role_by_name()
- roles.py
- PurchasePlan
- timedelta
- AdManager
- FreeRole
- TestMetadataPresets
- FirebaseService
- AdminRole
- MainWindow
- CacheProcessor
- ._update_video_list()
- patch
- test_youtube_upload_blocking.py
- PurchaseService
- patch
- test_session.py
- UsageTracker
- SelectionScreen
- LoginScreen
- SupabaseService
- ArrangementScreen
- get_youtube_service()
- PremiumRole
- ._upload_to_youtube()
- test_video_processor.py
- patch
- Role
- GuestRole
- ._close_dialog()
- SaveUploadScreen
- test_usage_tracker.py
- admin_audit_logs Firestore collection
- YouTubeUploader
- patch
- test_session_purchase.py
- .build()
- .get_remaining_arrangements()
- CacheSettings
- TestPurchaseServiceInitialization
- AuditLogService
- TestPurchasePlans
- UsageConfig
- metadata.py
- Software Requirements Specification v1.0
- firebase_service.py
- ConfigTab
- VideoMetadata
- uploader.py
- test_cache_processor.py
- Cloud-Stored Metadata Presets (Firestore)
- Video Merger and Uploader
- ._cache_thread()
- TestAuditLogRetrieval
- TestCacheDiagnosis
- ._show_error()
- TestGuestRole
- AuditLogViewer component (documented)
- RoleLimits
- ._show_upload_premium_message()
- TestRoleManager
- TestUsageTrackerFreeUsers
- TestUsageTrackerEdgeCases
- Initial Wireframe (low-fidelity UI
- RoleManager
- fixture
- TestFreeRole
- ._save_preset_to_database()
- test_cache_diagnosis.py
- TestDownscaleCalculations
- TestAdminFunctions
- TestMergeOtherClipsButton
- TestTransactionRetrieval
- TestTransactionDetails
- TestPermissionChecking
- TestSessionManagerInitialization
- TestUsageInfoDisplay
- TestArrangementChangeIndicator
- TestPremiumFeatureIndicators
- TestColorCoding
- TestUploadButtonState
- TestPremiumUpsellDialog
- Layered Architecture (Presentation /
- test_ui_feedback.py
- test_drag_drop_restrictions.py
- ._get_date_range()
- TestScopeConfiguration
- test_disable_user.py
- TestPlaceholderUserCreation
- TestUserRetrieval
- TestRoleManagement
- TestAuditLogging
- TestFirebaseServiceInitialization
- TestUserCreation
- TestArrangementScreenGuestLockout
- TestGuestArrangementControls
- TestButtonFunctionality
- TestUserWorkflow
- TestButtonPlacement
- TestEdgeCases
- TestButtonAccessibility
- TestPermission
- TestRoleUpdate
- TestErrorHandlingIntegration
- TestRobustnessScenarios
- TestAccuracyVerification
- TestUsageWarnings
- TestUploadButtonFeedback
- TestAdBanner
- TestUsageTrackerPremiumUsers
- TestUsageTrackerDailyReset
- TestUsageTrackerInitialization
- TestTimeParsingFromFFmpeg
- TestFFmpegAvailability
- TestUploadButtonClick
- TestMetadataPresetsIntegration
- ._apply_template()
- fresh_tracker()
- Multi-Role System (Guest /
- ._initialize_firebase()
- .set_videos()
- TestAuditLogIntegration
- TestPremiumDragDropAccess
- TestUsageTracking
- TestUserDeletion
- TestGetAuditLogs
- TestGuestLoginPrompt
- TestAuthenticatedUserComparison
- TestButtonAlternatives
- TestStateReset
- TestUIConsistency
- TestRoleType
- TestLogout
- TestUserDisplayInfo
- TestMainWindowIntegration
- TestSnackbarNotifications
- TestProgressiveDisclosure
- TestAccessibility
- TestUsageTrackerPersistence
- TestUploadStatusMessage
- TestUploadButtonIcon
- TestUploadWorkflow
- TestSaveStillWorks
- TestUIFeedback
- TestIntegrationUploadBlocking
- TestPremiumFeatureMessaging
- TestEdgeCases
- YouTube Data API v3
- .test_build_youtube_service_with_valid_creds()
- .test_get_user_info_from_credentials()
- TestStepIndicatorForGuest
- test_same_codec_preview()
- Flet 0.28.3 GUI framework
- app/__init__.py
- conftest.py
- videomerger-app

## God Nodes (most connected - your core abstractions)
1. `SaveUploadScreen` - 147 edges
2. `ArrangementScreen` - 101 edges
3. `FreeRole` - 70 edges
4. `SessionManager` - 66 edges
5. `AdminDashboard` - 50 edges
6. `ConfigTab` - 45 edges
7. `UsageTracker` - 44 edges
8. `MainWindow` - 42 edges
9. `FirebaseService` - 41 edges
10. `PurchaseService` - 28 edges

## Surprising Connections (you probably didn't know these)
- `Smart Video Processing with Intelligent Caching` --semantically_similar_to--> `Smart Codec Detection (stream copy vs re-encode)`  [INFERRED] [semantically similar]
  docs/VideoMergerandUploaderDocu.pdf → README.md
- `Micro-Analytics with Automated Usage Tracking` --semantically_similar_to--> `Usage Tracking & Daily Limits`  [INFERRED] [semantically similar]
  docs/VideoMergerandUploaderDocu.pdf → README.md
- `Offline Queue (future enhancement)` --semantically_similar_to--> `Offline-First Strategy (queued uploads, pending)`  [INFERRED] [semantically similar]
  docs/VideoMergerandUploaderDocu.pdf → README.md
- `Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99)` --conceptually_related_to--> `PurchasePlan`  [AMBIGUOUS]
  docs/PREMIUM_PURCHASE_IMPLEMENTATION.md → src/access_control/purchase_service.py
- `Multi-Role System (Guest / Free / Premium / Admin)` --conceptually_related_to--> `FreeRole`  [AMBIGUOUS]
  README.md → src/access_control/roles.py

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Admin multi-layer security (UI check, backend verify, Firestore rules, audit log, rate limit)** — videomerger_app_readme_defense_in_depth_strategy, videomerger_app_src_access_control_session_sessionmanager_has_permission, videomerger_app_src_access_control_firebase_service_firebaseservice_verify_admin_permission, videomerger_app_docs_admin_dashboard_todo_recommended_firestore_security_rules, videomerger_app_src_access_control_firebase_service_firebaseservice_log_admin_action, videomerger_app_src_access_control_firebase_service_firebaseservice_check_rate_limit, videomerger_app_docs_admin_dashboard_todo_application_level_security_model [EXTRACTED 1.00]
- **Audit log pipeline: log_admin_action -> admin_audit_logs -> get_audit_logs -> viewer -> CSV export** — videomerger_app_src_access_control_firebase_service_firebaseservice_log_admin_action, videomerger_app_docs_audit_logging_guide_admin_audit_logs_collection, videomerger_app_src_access_control_firebase_service_firebaseservice_get_audit_logs, videomerger_app_docs_audit_log_viewer_implementation_auditlogviewer_component, videomerger_app_src_app_gui_audit_log_viewer_auditlogservice, videomerger_app_docs_audit_log_quick_reference_audit_log_csv_export [INFERRED 0.85]
- **Freemium tier gating: role system, daily arrangement quota, upload block, premium purchase** — videomerger_app_readme_multi_role_system, videomerger_app_docs_access_levels_guide_free_user_daily_arrangement_limit, videomerger_app_src_access_control_usage_tracker_usagetracker, videomerger_app_docs_new_features_test_summary_youtube_upload_blocking_for_free_users, videomerger_app_docs_premium_purchase_implementation_premium_purchase_flow, videomerger_app_src_access_control_purchase_service_purchaseservice, videomerger_app_docs_videomergeranduploaderdocu_user_capabilities_matrix [INFERRED 0.85]

## Communities (161 total, 3 thin omitted)

### Community 0 - "AdminDashboard"
Cohesion: 0.06
Nodes (32): Admin Dashboard Tabs (User Management / Audit Logs), AdminDashboard, Any, Page, Update the audit logs table with current data, Export audit logs to CSV, Clear all audit log filters, Build the user management section with inline audit log viewer (+24 more)

### Community 1 - "SessionManager"
Cohesion: 0.04
Nodes (27): Known Test Failures (get_user_display_info, OAuth mock paths, role-name validation), Manages user session and role state throughout the app with Firebase integration, Update user role (for purchases, upgrades, etc.), Lazy load Firebase service to avoid import issues, Increment merge count in Firebase, Increment upload count in Firebase, Clear user session and optionally clear OAuth tokens, Clear OAuth token files (+19 more)

### Community 2 - ".create_role_by_name()"
Cohesion: 0.06
Nodes (37): Create a role instance by name string, mock_firebase_service(), mock_user_info(), mock_youtube_service(), fixture, patch, Integration tests for Authentication Flow Tests full authentication workflow:…, Test user management operations through full stack (+29 more)

### Community 3 - "roles.py"
Cohesion: 0.07
Nodes (34): Config, Configuration management for the app, Application configuration, get_firebase_service(), Get the global Firebase service instance, Access Control Module Backward compatibility imports for the access control…, Permission, Enum (+26 more)

### Community 4 - "PurchasePlan"
Cohesion: 0.05
Nodes (29): PurchasePlan, PurchaseStatus, Enum, Mock Purchase Service for Premium Upgrades Simulates a payment API for…, Status of a purchase transaction, Available premium plans, Tests for Purchase Service - Mock Premium Purchase API Tests premium…, Test that each transaction gets unique ID (+21 more)

### Community 5 - "timedelta"
Cohesion: 0.07
Nodes (28): timedelta, Test that get_audit_logs performs client-side filtering to avoid Firestore…, test_get_audit_logs_client_side_filtering(), Test that successful purchase sets correct premium expiration (100 years), patch, Test that role is upgraded correctly after purchase, Test that free user becomes premium after purchase, Test that premium permissions are granted after purchase (+20 more)

### Community 6 - "AdManager"
Cohesion: 0.07
Nodes (22): Mock Payment & Ad Services, AdConfig, AdManager, Page, Ad Manager - Handles ad rotation, timing, and Image-based ad display Uses…, Move to next vertical ad and return it, Register a callback to be called when ad should update, Unregister an update callback (+14 more)

### Community 7 - "FreeRole"
Cohesion: 0.07
Nodes (24): FreeRole, Free tier user - can save but cannot upload to YouTube, Test that non-guest users are stored as last user, Test login with auth token, Test usage tracking methods, Test incrementing merge count (no errors), Test incrementing upload count (no errors), Test session property accessors (+16 more)

### Community 8 - "TestMetadataPresets"
Cohesion: 0.06
Nodes (20): fixture, Test retrieving presets when user has none, Test metadata preset operations, Test getting presets when Firebase is unavailable, Test updating a preset, Create a mock Firestore client, Test updating preset when Firebase is unavailable, Test deleting a preset (+12 more)

### Community 9 - "FirebaseService"
Cohesion: 0.07
Nodes (19): FirebaseService, Any, Create a placeholder user document for a user who hasn't logged in yet This…, Firebase Admin SDK service for user and role management, Get user document by email, Get user document by UID, Update user's last login timestamp by UID or email, Increment user's usage count (+11 more)

### Community 10 - "AdminRole"
Cohesion: 0.07
Nodes (23): AdminRole, Admin role - all permissions including user management, fixture, Unit tests for Role Management System Tests role creation, permissions, and…, Create an admin role for testing, Test that admin has all permissions, Test that admin has user management permissions, Test that admin can view analytics (+15 more)

### Community 11 - "MainWindow"
Cohesion: 0.08
Nodes (20): MainWindow, Navigate to specific step, Move to next wizard step, Move to previous wizard step, Main application window with stepper navigation, Handle next button click - delegate to current screen, Handle back button click - delegate to current screen, Build and return the main layout (+12 more)

### Community 12 - "CacheProcessor"
Cohesion: 0.07
Nodes (19): CacheProcessor, Cache Processor - Handles incremental video caching with downscaling Supports…, Check if videos have different codecs, resolutions, or framerates. Stream copy…, Handles video caching with downscaling and preview-friendly format, Clear old cache files, Clear ALL cached files immediately, Cancel current caching operation, Create cached merged video with downscaling Intelligently decides whether to… (+11 more)

### Community 13 - "._update_video_list()"
Cohesion: 0.07
Nodes (17): Arrangement Change Detection (quota only on real reorder), Guest Arrangement Lockout Overlay, Build and return arrangement screen layout (Frame 2), Select a video for preview, Handle when a video is dropped on another video, Visual feedback when hovering over a drop target, Remove visual feedback when drag leaves the target, Move video with respect to locked positions (+9 more)

### Community 14 - "patch"
Cohesion: 0.07
Nodes (22): patch, Test that free users at limit cannot use drag and drop, Free users who hit daily limit should not be able to drag, Free users who hit daily limit should not be able to drop, Free users with remaining arrangements should be able to drag, Test that admin users have unrestricted drag and drop, Admin users should always be able to drag, Test that drag and drop cannot bypass arrangement limits (+14 more)

### Community 15 - "test_youtube_upload_blocking.py"
Cohesion: 0.09
Nodes (27): Free User Daily Arrangement Limit, Guest Arrangement Skip (step 0 -> step 2), New Features Test Suite (6 files, 245+ tests), YouTube Upload Blocking for Free Users (premium upsell), User Capabilities Matrix (Guest / Free / Premium / Admin), Quick Test Execution Guide (new feature tests), mock_page(), mock_session_free() (+19 more)

### Community 16 - "PurchaseService"
Cohesion: 0.09
Nodes (20): Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99), Premium Purchase Flow (upsell -> plan -> role upgrade -> Firebase sync), Purchase Test Suite (61 tests), Premium Purchase System (mock, lifetime PHP 5.00), get_purchase_service(), PurchaseService, Any, Create a successful transaction record (+12 more)

### Community 17 - "patch"
Cohesion: 0.08
Nodes (20): patch, Test video dimension detection, Test successful dimension detection, Test that default dimensions are returned on failure, Test timeout handling in dimension detection, Test cache creation functionality, Test cache creation with empty video list, Test that create_cache runs in background thread (+12 more)

### Community 18 - "test_session.py"
Cohesion: 0.09
Nodes (26): Core Test Suite (124 tests, 104 passing, 83.9%), Testing & Quality Assurance (pytest, claimed 100+ tests), pytest==9.0.1, Unit tests for OAuth Authentication Tests OAuth token handling and YouTube…, Test token saving functionality, Test handling of corrupted token files, TestCorruptedTokenHandling, TestTokenSaving (+18 more)

### Community 19 - "UsageTracker"
Cohesion: 0.10
Nodes (18): usage_tracking.json local usage store, Tracks daily arrangement usage for users Features: - Tracks arrangement count…, Create storage directory if it doesn't exist, Load usage data from file, UsageTracker, Test that guest arrangements are not tracked, Test that guest arrangements are not recorded in usage tracker, Test that guest has 0 remaining arrangements (+10 more)

### Community 20 - "SelectionScreen"
Cohesion: 0.11
Nodes (14): FilePickerResultEvent, Page, Configure page settings, Show formatted welcome message, Page, Show premium purchase dialog, First screen: File selection with FilePicker, Prompt guest to login before purchasing (+6 more)

### Community 21 - "LoginScreen"
Cohesion: 0.11
Nodes (13): LoginScreen, Page, Login screen with guest and Google login options and Firebase integration, Handle guest login (local only, no database), Handle Google OAuth login with Firebase integration, Build and return the login screen UI, Show/hide loading indicator for Google login, Show/hide loading indicator for guest login (+5 more)

### Community 22 - "SupabaseService"
Cohesion: 0.10
Nodes (15): Client, get_supabase_service(), Any, Supabase Service Handles metadata presets and other SQL-based data storage, Update a metadata preset, Delete a metadata preset, Supabase service for preset management and data storage, Get or create Supabase service singleton (+7 more)

### Community 23 - "ArrangementScreen"
Cohesion: 0.10
Nodes (14): ArrangementScreen, Second screen: Arrange clips and preview, Sort videos while respecting locked positions, Clear old preview cache files when videos change, Show coming soon message for premium feature, Test tooltips and help text, Test that premium features show appropriate tooltips, Test that usage info has helpful explanatory text (+6 more)

### Community 24 - "get_youtube_service()"
Cohesion: 0.11
Nodes (17): get_youtube_service(), Authenticate and return a YouTubeService object. Loads token.pickle if…, patch, Test token refresh functionality, Test successful token refresh, Test token refresh failure triggers reauth, Test OAuth flow uses default port 8080, Test OAuth flow falls back to alternative ports on failure (+9 more)

### Community 25 - "PremiumRole"
Cohesion: 0.09
Nodes (16): PremiumRole, Premium user - full features, no ads, Create a premium role for testing, Test that premium has all basic permissions, Test that premium has premium features, Test that premium has no limits, Test that role hierarchy is properly enforced, Test that admin has most permissions (+8 more)

### Community 26 - "._upload_to_youtube()"
Cohesion: 0.10
Nodes (12): Confirm and start merge + upload process, Start YouTube upload process, Upload merged video to YouTube using uploader module, Lazy load video processor, Merge videos for preview (cached in background with downscaling), Handle save button click - show confirmation with final settings, Merge videos for final save, Handle upload button - save and upload to YouTube (+4 more)

### Community 27 - "test_video_processor.py"
Cohesion: 0.09
Nodes (19): output_path(), fixture, Tests for Video Processor - FFmpeg video merging functionality, Create a VideoProcessor instance for testing, Create sample video file paths for testing, Test process control functionality, Test canceling current processing, Test that processing state is tracked correctly (+11 more)

### Community 28 - "patch"
Cohesion: 0.10
Nodes (16): patch, Test video duration calculation, Test successful duration calculation, Test handling when duration cannot be calculated, Test that ffprobe command is formatted correctly, Test video merging functionality, Test merging with empty video list, Test that merge_videos creates a background thread (+8 more)

### Community 29 - "Role"
Cohesion: 0.09
Nodes (14): get_role(), Get a role instance by name (convenience function), Base role class with permissions and limitations, Check if role has specific permission, Check if role has any of the specified permissions, Check if role has all of the specified permissions, Check if role can perform a specific action by name, Role (+6 more)

### Community 30 - "GuestRole"
Cohesion: 0.10
Nodes (16): GuestRole, Guest role - limited features and ads, Test that guest has fewest permissions, Test basic purchase_premium functionality, Test that purchase_premium method exists, Test that purchase fails when user not logged in, Test that guest users cannot purchase premium, TestPurchasePremiumBasics (+8 more)

### Community 31 - "._close_dialog()"
Cohesion: 0.11
Nodes (12): Show upload success dialog, Show upload error dialog, Retry upload after error, Show premium purchase dialog with plan options, Prompt guest to login before purchasing, Close dialog and trigger login flow, Start a new merge - go back to selection screen, Show confirmation dialog with final merge settings (+4 more)

### Community 32 - "SaveUploadScreen"
Cohesion: 0.11
Nodes (13): Show upgrade message using snack bar, Update progress for preview merge, Handle preview merge completion - display the cached video, Third screen: Configure output and upload settings, Monitor cache file and update preview once it has content, Display the preview video, Open directory picker for output location, SaveUploadScreen (+5 more)

### Community 33 - "test_usage_tracker.py"
Cohesion: 0.09
Nodes (17): mock_session_manager(), fixture, Unit tests for usage tracker - daily arrangement limits for free users Tests…, Create temporary storage directory for tests, Test usage tracking for admin users, Test that admin users have unlimited arrangements, Test that admin users can always arrange, Test usage tracking for guest users (+9 more)

### Community 34 - "admin_audit_logs Firestore collection"
Cohesion: 0.16
Nodes (19): admin_audit_logs composite index (timestamp, admin_email, action), Admin Dashboard TODO Tracker, Application-level Security Model (Admin SDK bypasses rules), Audit Log Retention Policy (90-day Cloud Function cleanup), First Admin Bootstrap (Config.SUPER_ADMIN_EMAIL), Admin Rate Limiting (sliding window, not implemented), Re-authentication for Critical Admin Actions (TODO), Recommended Firestore Security Rules (isAdmin, future web deployment) (+11 more)

### Community 35 - "YouTubeUploader"
Cohesion: 0.11
Nodes (12): Any, Build the request body for YouTube API., Container for all upload settings, Get the status of an uploaded video., Process the upload queue with progress tracking., Apply metadata template to a video., Save upload progress to disk (optional)., Handles YouTube video uploads without GUI (+4 more)

### Community 36 - "patch"
Cohesion: 0.12
Nodes (12): patch, Test Admin Dashboard Integration Ensures proper initialization order and no…, Test that ConfigTab uses real AdminDashboard without duplicate logic, Test correct initialization order of admin dashboard, Test that duplicate _admin_* methods are removed from ConfigTab, Test the correct execution order of admin dashboard methods, Test that build() creates UI components before load_users() is called, Test that calling load_users() before build() causes an error (+4 more)

### Community 37 - "test_session_purchase.py"
Cohesion: 0.11
Nodes (17): clean_session(), logged_in_free_user(), mock_firebase(), mock_purchase_service(), fixture, Tests for Session Manager Premium Purchase Integration Tests the…, Clean session for each test, Session with logged in free user (+9 more)

### Community 38 - ".build()"
Cohesion: 0.13
Nodes (10): Build config tab for authenticated users with toggle back to admin dashboard, Build config tab for guest users (no YouTube access), Build the integrated admin dashboard using the real AdminDashboard class, Build account information section, Build metadata templates section with presets, Build app settings section, Get available template options, Build and return config tab layout based on user role (+2 more)

### Community 39 - ".get_remaining_arrangements()"
Cohesion: 0.16
Nodes (10): datetime, Get remaining arrangements for current user Returns: int: Remaining…, Check if current user can arrange videos Returns: bool: True if user can…, Record an arrangement usage Returns: bool: True if recorded successfully, False…, Get formatted string of when the limit resets, Get detailed usage information for current user Returns: dict: Usage…, Save usage data to file, Get unique key for current user (+2 more)

### Community 40 - "CacheSettings"
Cohesion: 0.13
Nodes (11): CacheSettings, Settings for video caching and downscaling, Test FFmpeg command construction for caching, Test FFmpeg command with downscaling enabled, Test FFmpeg command without downscaling, Test that command includes parameters for consistent output, Test CacheSettings configuration, Test default cache settings (+3 more)

### Community 41 - "TestPurchaseServiceInitialization"
Cohesion: 0.12
Nodes (13): Reset the global purchase service instance (mainly for testing), reset_purchase_service(), mock_user_email(), purchase_service(), fixture, Create a fresh purchase service for testing, Mock user email for testing, Test purchase service initialization (+5 more)

### Community 42 - "AuditLogService"
Cohesion: 0.16
Nodes (10): AuditLogService, Service for fetching and exporting audit logs, Verify user has permission to view audit logs, Test Audit Log Viewer UI component, Test audit log viewer initialization with proper permissions, Test audit log viewer blocks unauthorized access, Test loading and displaying audit logs, Test filter controls trigger log reload (+2 more)

### Community 43 - "TestPurchasePlans"
Cohesion: 0.13
Nodes (9): Get information about a premium plan Args: plan: Plan to get info for Returns:…, Get information about all available plans, Test that all plans have features listed, Test purchase plan configuration, Test lifetime plan has correct price, Test lifetime plan duration (100 years), Test get_plan_info returns all plan details, Test get_all_plans returns single lifetime plan (+1 more)

### Community 44 - "UsageConfig"
Cohesion: 0.12
Nodes (11): Configuration for usage limits, UsageConfig, Test daily reset behavior in integrated system, Test that all users get reset at midnight, Test that reset time info is accurate, TestDailyResetIntegration, Test get_usage_info method, Test usage info for free user (+3 more)

### Community 45 - "metadata.py"
Cohesion: 0.17
Nodes (14): build_metadata_from_form(), generate_metadata(), load_template(), _parse_tags(), Metadata Module Handles loading and generating video metadata for uploads., Generate and save a metadata template file for reuse., Strongly typed metadata structure for uploads., Load metadata template from JSON or YAML file. (+6 more)

### Community 46 - "Software Requirements Specification v1.0"
Cohesion: 0.17
Nodes (15): ISO/IEC/IEEE 29148:2018 (Requirements engineering), Long-Term SRS (LTSRS) v1.0, Oct 6 2025, LTSRS NFR-003: tokens encrypted and stored locally, LTSRS NFR-004: recover from upload interruptions, store logs locally, FR-005 Progress Tracking and Notifications, FR-006 Error Handling and Logging, NFR-001 Performance (10 HD clips < 5 min, upload feedback < 5 s), NFR-002 Usability (merge+upload within 3 attempts) (+7 more)

### Community 47 - "firebase_service.py"
Cohesion: 0.14
Nodes (12): datetime, Firebase Admin SDK Service Handles user management, role assignments, and…, Set user's premium expiration date, # TODO: Log to audit trail, # TODO: Log to audit trail, # TODO: Archive user data first, # TODO: Delete from Firebase Auth, # TODO: Log to audit trail (+4 more)

### Community 48 - "ConfigTab"
Cohesion: 0.15
Nodes (7): ConfigTab, Show available presets in a dialog for selection, Config tab for app settings and metadata templates, Clear all template fields, Browse for output directory, Browse for FFmpeg executable, Load presets from Firebase database

### Community 49 - "VideoMetadata"
Cohesion: 0.18
Nodes (8): Check if metadata was extracted successfully, Get formatted display text for UI, Get short metadata info (codec, resolution, fps), Video metadata information, Check if this video has compatible properties with another, Get list of compatibility issues with another video, Extract video metadata using ffprobe, VideoMetadata

### Community 50 - "uploader.py"
Cohesion: 0.14
Nodes (10): YouTube Auth Module Handles OAuth 2.0 authentication for Google APIs., Wrapper for YouTube API service and credentials., YouTubeService, YouTube Uploader Module Handles all non-GUI video upload logic, # TODO: Upload each video, update progress bars, # TODO: Use template system for title/description/tags, # TODO: Write progress to file, Test YouTubeService wrapper class (+2 more)

### Community 51 - "test_cache_processor.py"
Cohesion: 0.16
Nodes (13): cache_path(), cache_processor(), cache_settings(), fixture, Tests for Cache Processor - Downscaled video caching functionality, Create cache settings for testing, Create a CacheProcessor instance for testing, Create sample video file paths for testing (+5 more)

### Community 52 - "Cloud-Stored Metadata Presets (Firestore)"
Cohesion: 0.22
Nodes (10): Firebase project video-merger-edc29, metadata_presets composite index (user_id ASC, created_at DESC), Cloud-Stored Metadata Presets (Firestore), metadata_presets Firestore collection, Metadata Templates & Presets (local JSON + Firestore), Create a metadata preset for a user Args: user_id: User's email or identifier…, Get all metadata presets for a user Args: user_id: User's email or identifier…, Delete a metadata preset Args: preset_id: Document ID of the preset Returns:… (+2 more)

### Community 53 - "Video Merger and Uploader"
Cohesion: 0.21
Nodes (14): FR-003 Video Merging (FFmpeg, output format/resolution), Video Merger and Uploader Course Documentation (AppDev + IAS), Fragmented Content-Creation Workflow (problem statement), Group 7 Team (Bacsain 50%, Parro 20%, Prestado 30%), Smart Video Processing with Intelligent Caching, Offline Queue (future enhancement), Application Development & Emerging Technologies course, FFmpeg (+6 more)

### Community 54 - "._cache_thread()"
Cohesion: 0.14
Nodes (7): Internal thread function for caching, Build FFmpeg command for caching - FAST stream copy for same-codec videos This…, Calculate downscaled dimensions maintaining aspect ratio, Get video width and height, Create temporary concat file for FFmpeg, Get total duration of all videos in seconds, Parse current time from FFmpeg stderr output

### Community 55 - "TestAuditLogRetrieval"
Cohesion: 0.14
Nodes (8): Test filtering logs by date range, Test filtering logs with multiple criteria, Test audit log retrieval with various filters, Test retrieving all audit logs without filters, Test filtering logs by actor (admin email), Test filtering logs by action type, Test filtering logs by target user, TestAuditLogRetrieval

### Community 56 - "TestCacheDiagnosis"
Cohesion: 0.14
Nodes (8): Test total duration calculation, Test actual cache creation with timing, Test concat file is properly formatted, Diagnostic tests for cache processor, Test that FFmpeg command is properly structured, Test video dimension detection, Test downscale dimension calculation, TestCacheDiagnosis

### Community 57 - "._show_error()"
Cohesion: 0.18
Nodes (6): Handle template selection, Save current template with confirmation dialog, Load template from file picker, Load template by name from templates directory, Populate template fields with data, Delete selected template

### Community 58 - "TestGuestRole"
Cohesion: 0.15
Nodes (7): Test guest file size limit, Create a guest role for testing, Test that guest has basic permissions, Test that guest cannot upload videos, Test that guest doesn't have premium features, Test guest video length limit, TestGuestRole

### Community 59 - "AuditLogViewer component (documented)"
Cohesion: 0.30
Nodes (10): Audit Log Viewer Implementation Summary (feature/audit-log), Audit Log CSV Export (storage/exports/audit_logs_*.csv), Audit Log Viewer Quick Reference, Audit Log Multi-Filter (actor, target user, action type, date range), AuditLogViewer component (documented), Admin Dashboard (user and role management), Enhancement 4: Audit Log Viewer, Information Assurance & Security course (+2 more)

### Community 60 - "RoleLimits"
Cohesion: 0.24
Nodes (6): Defines limits for each role, RoleLimits, Test RoleLimits dataclass, Test default limit values, Test creating custom limits, TestRoleLimits

### Community 61 - "._show_upload_premium_message()"
Cohesion: 0.18
Nodes (6): Show premium purchase dialog, Show message that upload is a premium feature, Build and return save/upload screen layout, Build video list display with metadata, Update upload button state after role change, Get user-friendly role display text

### Community 62 - "TestRoleManager"
Cohesion: 0.17
Nodes (7): Test RoleManager factory, Test creating guest role by name, Test creating free role by name, Test creating premium role by name, Test creating admin role by name, Test that invalid role name raises ValueError, TestRoleManager

### Community 63 - "TestUsageTrackerFreeUsers"
Cohesion: 0.17
Nodes (7): Test that recording arrangement decrements counter, Test that free user cannot arrange after reaching limit, Test recording multiple arrangements, Test usage tracking for free users, Test that free user can arrange when starting fresh, Test that free user has correct daily limit, TestUsageTrackerFreeUsers

### Community 64 - "TestUsageTrackerEdgeCases"
Cohesion: 0.17
Nodes (7): Test edge cases and error handling, Test handling when user key cannot be determined, Test handling of corrupted usage file, Test that user key is extracted from email, Test that user key falls back to uid if no email, Test that different users are tracked separately, TestUsageTrackerEdgeCases

### Community 65 - "Initial Wireframe (low-fidelity UI"
Cohesion: 0.22
Nodes (11): Access Level System (arrangement gating by role), Premium Video Position Lock, FR-002 Video Selection and Arrangement, Arrange-By Sort Menu (name / date / length, asc / desc), Initial Wireframe (low-fidelity UI mockups), Save/Upload button reserved for Premium Users, Wireframe Stepper: Select Videos -> Merge -> Save/Upload, Watermark Feature (VideoCompiler watermark, user watermark, Remove Watermark Premium) (+3 more)

### Community 66 - "RoleManager"
Cohesion: 0.22
Nodes (7): Design patterns: Singleton / Factory / Strategy, Manages role creation and validation, Create a role instance by type, Get instances of all available roles, Get roles ordered by privilege level (least to most), Check if changing from one role to another is an upgrade, RoleManager

### Community 67 - "fixture"
Cohesion: 0.18
Nodes (6): fixture, Create a mock Flet page, Mock session manager with admin permissions, Mock Firebase service, Create a mock Firebase service, Sample audit log data

### Community 68 - "TestFreeRole"
Cohesion: 0.18
Nodes (6): Create a free role for testing, Test that free users can upload videos, Test that free has basic permissions, Test that free users still see ads, Test free video length limit, TestFreeRole

### Community 69 - "._save_preset_to_database()"
Cohesion: 0.20
Nodes (5): Handle clicks on title for admin access (hidden button), Test FFmpeg installation, Save application settings, Show success snackbar, Save current template as a preset to Firebase database

### Community 70 - "test_cache_diagnosis.py"
Cohesion: 0.24
Nodes (9): cache_processor(), cache_settings(), fixture, Diagnostic tests for cache processor to identify duration and performance issues, # NOTE: Stream copy mode may have timestamp issues causing incorrect duration…, Fixture providing paths to test videos, Fixture providing cache settings, Fixture providing cache processor instance (+1 more)

### Community 71 - "TestDownscaleCalculations"
Cohesion: 0.20
Nodes (6): Test that odd dimensions are rounded to even numbers, Test various downscale factors, Test video downscaling dimension calculations, Test 50% downscaling calculation, Test downscaling when disabled, TestDownscaleCalculations

### Community 72 - "TestAdminFunctions"
Cohesion: 0.20
Nodes (6): Test admin-specific functions, Test retrieving all users, Test admin verification for admin user, Test admin verification for non-admin user, Test admin verification when user not found, TestAdminFunctions

### Community 73 - "TestMergeOtherClipsButton"
Cohesion: 0.20
Nodes (6): Test 'Merge Other Clips' button in success dialogs, Test that button appears in save success dialog, Test that button appears in upload success dialog, Test that button has video library icon, Test that button has correct styling (blue elevated button), TestMergeOtherClipsButton

### Community 74 - "TestTransactionRetrieval"
Cohesion: 0.20
Nodes (6): Test transaction lookup and retrieval, Test retrieving transaction by ID, Test that invalid transaction ID returns None, Test retrieving all transactions for a user, Test that new user has no transactions, TestTransactionRetrieval

### Community 75 - "TestTransactionDetails"
Cohesion: 0.20
Nodes (6): Test transaction data structure and details, Test that transaction has all required fields, Test that purchased_at timestamp is recent, Test that transaction ID has expected format, Test that currency is PHP, TestTransactionDetails

### Community 76 - "TestPermissionChecking"
Cohesion: 0.20
Nodes (6): Test permission checking methods, Test that guest cannot upload videos, Test that free user can upload videos, Test permission checking when not logged in, Test that admin has user management permission, TestPermissionChecking

### Community 77 - "TestSessionManagerInitialization"
Cohesion: 0.20
Nodes (6): Test SessionManager initialization, Test that session starts in logged out state, Test that session doesn't start as guest, Test that session has no email initially, Test that session has no uid initially, TestSessionManagerInitialization

### Community 78 - "TestUsageInfoDisplay"
Cohesion: 0.20
Nodes (6): Test that premium users don't see usage counter, Test that usage counter updates when arrangement changes, Test usage info display in arrangement screen, Test that free users see usage counter, Test that usage counter shows correct format, TestUsageInfoDisplay

### Community 79 - "TestArrangementChangeIndicator"
Cohesion: 0.20
Nodes (6): Test the change indicator for arrangements, Test that orange indicator appears when arrangement changes, Test that change indicator is hidden when no changes made, Test that free users see trial usage warning in indicator, Test that premium users see different indicator message, TestArrangementChangeIndicator

### Community 80 - "TestPremiumFeatureIndicators"
Cohesion: 0.20
Nodes (6): Test premium feature UI indicators, Test that premium users see lock feature indicator, Test that free users don't see lock feature indicator, Test that lock/unlock buttons are visible for premium users, Test that lock/unlock buttons are hidden for free users, TestPremiumFeatureIndicators

### Community 81 - "TestColorCoding"
Cohesion: 0.20
Nodes (6): Test color coding for different states, Test usage counter color when usage is normal, Test usage counter color when limit is approaching, Test usage counter color when limit is reached, Test that change indicator is orange, TestColorCoding

### Community 82 - "TestUploadButtonState"
Cohesion: 0.20
Nodes (6): Test upload button state for different users, Test that free users see locked upload button, Test that premium users see enabled upload button, Test that guest users see locked upload button, Test that free users see premium upsell tooltip, TestUploadButtonState

### Community 83 - "TestPremiumUpsellDialog"
Cohesion: 0.20
Nodes (6): Test premium upsell dialog content and behavior, Test that premium dialog shows premium features, Test that premium dialog has upgrade button, Test that premium dialog can be dismissed, Test that upgrade button shows coming soon message, TestPremiumUpsellDialog

### Community 84 - "Layered Architecture (Presentation /"
Cohesion: 0.31
Nodes (9): FR-001 User Authentication (hybrid Google OAuth + Firebase, 4 roles), NFR-003 Security (pickled tokens, no stored passwords), Layered Architecture (Presentation / Business Logic / Data & Service / External), API credentials in configs/ (client_secret.json, firebase-admin-key.json), Firebase Auth + Firestore, Google OAuth 2.0, OWASP Top 10 Mitigation Mapping, token.pickle OAuth token storage (+1 more)

### Community 85 - "test_ui_feedback.py"
Cohesion: 0.28
Nodes (8): UI Feedback Indicators (usage counter, change indicator, color coding), mock_page(), mock_session_free(), mock_session_premium(), fixture, Unit and integration tests for UI feedback improvements Tests arrangement usage…, Mock session for free user, Mock session for premium user

### Community 86 - "test_drag_drop_restrictions.py"
Cohesion: 0.28
Nodes (8): mock_page(), mock_parent(), mock_videos(), fixture, Tests for Arrangement Drag and Drop Restrictions Ensures drag and drop respects…, Create mock Flet page, Create mock video list, Create mock parent window

### Community 87 - "._get_date_range()"
Cohesion: 0.25
Nodes (5): Any, datetime, Fetch audit logs from Firebase with filters, Get start and end dates based on range string, Export logs to CSV file. Returns (success, message)

### Community 88 - "TestScopeConfiguration"
Cohesion: 0.25
Nodes (5): Test OAuth scope configuration, Test that required YouTube upload scope is configured, Test that user info scopes are configured, Test that OpenID scope is configured, TestScopeConfiguration

### Community 89 - "test_disable_user.py"
Cohesion: 0.29
Nodes (4): admin_dashboard(), mock_page(), fixture, test_toggle_user_status_prevent_super_admin_disable()

### Community 90 - "TestPlaceholderUserCreation"
Cohesion: 0.25
Nodes (5): Test placeholder user creation, Test creating placeholder when Firebase is unavailable, Test creating placeholder for new user, Test creating placeholder for existing user updates role, TestPlaceholderUserCreation

### Community 91 - "TestUserRetrieval"
Cohesion: 0.25
Nodes (5): Test user retrieval methods, Test getting user by email when not found, Test getting user by email when found, Test getting user by UID, TestUserRetrieval

### Community 92 - "TestRoleManagement"
Cohesion: 0.25
Nodes (5): Test role update functionality, Test role update when Firebase unavailable, Test successful role update, Test upgrading from free to premium, TestRoleManagement

### Community 93 - "TestAuditLogging"
Cohesion: 0.25
Nodes (5): Test audit logging functionality, Test successful audit log creation, Test audit logging when Firebase unavailable, Test logging failed admin action, TestAuditLogging

### Community 94 - "TestFirebaseServiceInitialization"
Cohesion: 0.25
Nodes (5): Test Firebase service initialization, Test that service is unavailable without credentials, Test that service is available when properly mocked, Test that db property returns Firestore client, TestFirebaseServiceInitialization

### Community 95 - "TestUserCreation"
Cohesion: 0.25
Nodes (5): Test user creation functionality, Test creating user when Firebase is unavailable, Test successful user creation, Test creating user with premium subscription, TestUserCreation

### Community 96 - "TestArrangementScreenGuestLockout"
Cohesion: 0.25
Nodes (5): Test arrangement screen lockout overlay for guests, Test that guest users see lockout overlay on arrangement screen, Test that all arrangement buttons are disabled for guests, Test that authenticated users don't see lockout overlay, TestArrangementScreenGuestLockout

### Community 97 - "TestGuestArrangementControls"
Cohesion: 0.25
Nodes (5): Test that guest users cannot manipulate arrangement, Test that guest users cannot move videos up, Test that guest users cannot duplicate videos, Test that guest users cannot sort videos, TestGuestArrangementControls

### Community 98 - "TestButtonFunctionality"
Cohesion: 0.25
Nodes (5): Test that button navigates back to selection screen (step 0), Test that button resets the merge workflow, Test button click functionality, Test that clicking button closes the dialog, TestButtonFunctionality

### Community 99 - "TestUserWorkflow"
Cohesion: 0.25
Nodes (5): Test complete user workflows with button, Test workflow: save video -> click 'Merge Other Clips, Test workflow: upload video -> click 'Merge Other Clips, Test user can merge multiple times in sequence, TestUserWorkflow

### Community 100 - "TestButtonPlacement"
Cohesion: 0.25
Nodes (5): Test button placement in dialogs, Test that button is in dialog actions section, Test that button is in upload success dialog actions, Test that 'Done' button is still present alongside 'Merge Other Clips, TestButtonPlacement

### Community 101 - "TestEdgeCases"
Cohesion: 0.25
Nodes (5): Test edge cases for merge other clips feature, Test that button handles missing main_window gracefully, Test that button works even if no videos were merged, Test that dialog is properly closed before navigation, TestEdgeCases

### Community 102 - "TestButtonAccessibility"
Cohesion: 0.25
Nodes (5): Test button accessibility for all user types, Test that free users can click 'Merge Other Clips, Test that premium users can click 'Merge Other Clips, Test that guests can click 'Merge Other Clips, TestButtonAccessibility

### Community 103 - "TestPermission"
Cohesion: 0.25
Nodes (5): Test Permission enumeration, Test that basic permissions are defined, Test that feature permissions are defined, Test that admin permissions are defined, TestPermission

### Community 104 - "TestRoleUpdate"
Cohesion: 0.25
Nodes (5): Test role update functionality, Test upgrading from free to premium, Test that role update fails when not logged in, Test updating to admin role, TestRoleUpdate

### Community 105 - "TestErrorHandlingIntegration"
Cohesion: 0.25
Nodes (5): Test error handling in integrated system, Test that tracker handles corrupted session data, Test that missing usage file is created automatically, Test that concurrent access to usage data is handled, TestErrorHandlingIntegration

### Community 106 - "TestRobustnessScenarios"
Cohesion: 0.25
Nodes (5): Test system robustness under various conditions, Test handling of rapid arrangement changes, Test that usage persists across app restarts, Test that reset time handles timezone correctly, TestRobustnessScenarios

### Community 107 - "TestAccuracyVerification"
Cohesion: 0.25
Nodes (5): Verify accuracy of usage tracking, Test that counter is accurate for single user, Test that usage info is accurate, Test accuracy at edge of limit, TestAccuracyVerification

### Community 108 - "TestUsageWarnings"
Cohesion: 0.25
Nodes (5): Test usage limit warnings and notifications, Test that warning is shown when user is close to limit, Test notification when limit is reached, Test that reset time is shown in limit warning, TestUsageWarnings

### Community 109 - "TestUploadButtonFeedback"
Cohesion: 0.25
Nodes (5): Test upload button UI feedback, Test that upload button appears disabled for free users, Test that upload button appears enabled for premium users, Test that upload button tooltip explains restriction for free users, TestUploadButtonFeedback

### Community 110 - "TestAdBanner"
Cohesion: 0.25
Nodes (5): Test ad banner for free users, Test that ad banner is displayed for free users, Test that ad banner is hidden for premium users, Test that ad banner has link to upgrade, TestAdBanner

### Community 111 - "TestUsageTrackerPremiumUsers"
Cohesion: 0.25
Nodes (5): Test usage tracking for premium users, Test that premium users have unlimited arrangements, Test that premium users can always arrange, Test that premium user arrangements are not tracked, TestUsageTrackerPremiumUsers

### Community 112 - "TestUsageTrackerDailyReset"
Cohesion: 0.25
Nodes (5): Test daily reset functionality, Test that reset time is calculated correctly (next midnight), Test that usage resets after reset time passes, Test that reset doesn't trigger before reset time, TestUsageTrackerDailyReset

### Community 113 - "TestUsageTrackerInitialization"
Cohesion: 0.25
Nodes (5): Test usage tracker initialization and setup, Test that storage directory is created on init, Test that usage_data is empty dict on first run, Test that existing data is loaded correctly, TestUsageTrackerInitialization

### Community 114 - "TestTimeParsingFromFFmpeg"
Cohesion: 0.25
Nodes (5): Test parsing time from FFmpeg output, Test parsing HH:MM:SS.ms format, Test parsing different time formats, Test handling invalid time format, TestTimeParsingFromFFmpeg

### Community 115 - "TestFFmpegAvailability"
Cohesion: 0.25
Nodes (5): Test FFmpeg installation and availability, Test if FFmpeg is installed and accessible, Test handling when FFmpeg is not installed, Test FFmpeg version check command, TestFFmpegAvailability

### Community 116 - "TestUploadButtonClick"
Cohesion: 0.25
Nodes (5): Test upload button click behavior, Test that free users see premium upsell dialog when clicking upload, Test that premium users can upload when clicking button, Test that guests see premium upsell dialog when clicking upload, TestUploadButtonClick

### Community 117 - "TestMetadataPresetsIntegration"
Cohesion: 0.33
Nodes (5): integration, Integration tests for metadata presets (require actual Firebase connection), Test creating and retrieving preset with real Firebase, Test updating preset with real Firebase, TestMetadataPresetsIntegration

### Community 118 - "._apply_template()"
Cohesion: 0.29
Nodes (3): Cancel ongoing merge operation, Open dialog to edit upload settings, Apply a saved template to the upload form fields

### Community 119 - "fresh_tracker()"
Cohesion: 0.29
Nodes (7): clean_session(), fresh_tracker(), fixture, Create temporary storage for tests, Create a clean session manager, Create fresh usage tracker, temp_storage_dir()

### Community 120 - "Multi-Role System (Guest /"
Cohesion: 0.33
Nodes (6): Target User Personas (Content Creator, Streamer, Educator, Administrator), Micro-Analytics with Automated Usage Tracking, Multi-Role System (Guest / Free / Premium / Admin), Python/Firebase Access Control Integration (Pyrebase FirebaseAuth / UserSession), Usage Tracking & Daily Limits, Pyrebase4==4.8.0

### Community 121 - "._initialize_firebase()"
Cohesion: 0.33
Nodes (3): Initialize Firebase Admin SDK with service account key, Initialize Firebase Admin SDK, Get Firestore database client

### Community 122 - ".set_videos()"
Cohesion: 0.33
Nodes (3): Clean up old cache files from the cache directory, Show warning dialog for incompatible videos, Set videos and trigger preview merge

### Community 123 - "TestAuditLogIntegration"
Cohesion: 0.33
Nodes (4): Integration tests for audit logging system, Test that admin actions automatically create audit logs, Test that UI filters match backend query parameters, TestAuditLogIntegration

### Community 124 - "TestPremiumDragDropAccess"
Cohesion: 0.33
Nodes (4): Test that premium users have unrestricted drag and drop, Premium users should always be able to drag, Premium users should be able to drop videos unlimited times, TestPremiumDragDropAccess

### Community 125 - "TestUsageTracking"
Cohesion: 0.33
Nodes (4): Test usage tracking methods, Test incrementing usage count, Test updating last login timestamp, TestUsageTracking

### Community 126 - "TestUserDeletion"
Cohesion: 0.33
Nodes (4): Test user deletion functionality, Test successful user deletion, Test deletion when Firebase unavailable, TestUserDeletion

### Community 127 - "TestGetAuditLogs"
Cohesion: 0.33
Nodes (4): Test audit log retrieval, Test retrieving audit logs, Test retrieving logs when Firebase unavailable, TestGetAuditLogs

### Community 128 - "TestGuestLoginPrompt"
Cohesion: 0.33
Nodes (4): Test login prompts and navigation for guests, Test that guest can go back to selection screen to login, Test that guest can click 'Continue to Merge' button, TestGuestLoginPrompt

### Community 129 - "TestAuthenticatedUserComparison"
Cohesion: 0.33
Nodes (4): Compare guest vs authenticated user flows, Test that authenticated users can access arrangement screen, Test that authenticated users see arrangement controls, TestAuthenticatedUserComparison

### Community 130 - "TestButtonAlternatives"
Cohesion: 0.33
Nodes (4): Test button vs done button behavior, Test that 'Done' button only closes dialog without navigation, Test that 'Merge Other Clips' closes dialog AND navigates, TestButtonAlternatives

### Community 131 - "TestStateReset"
Cohesion: 0.33
Nodes (4): Test that state is properly reset for new merge, Test that selection screen is ready for new videos, Test that previous video selection doesn't carry over, TestStateReset

### Community 132 - "TestUIConsistency"
Cohesion: 0.33
Nodes (4): Test UI consistency across different dialogs, Test that button appears in both save and upload success dialogs, Test that button text is consistent across dialogs, TestUIConsistency

### Community 133 - "TestRoleType"
Cohesion: 0.33
Nodes (4): Test RoleType enumeration, Test that all role types have correct values, Test that we have exactly 5 role types, TestRoleType

### Community 134 - "TestLogout"
Cohesion: 0.33
Nodes (4): Test logout functionality, Test that logout clears session data, Test that logout preserves last user data, TestLogout

### Community 135 - "TestUserDisplayInfo"
Cohesion: 0.33
Nodes (4): Test user display information retrieval, Test getting user display info when logged in, Test getting user display info when logged out, TestUserDisplayInfo

### Community 136 - "TestMainWindowIntegration"
Cohesion: 0.33
Nodes (4): Test integration with main window flow, Test that main window checks usage before going to save screen, Test that usage is recorded when user saves arrangement, TestMainWindowIntegration

### Community 137 - "TestSnackbarNotifications"
Cohesion: 0.33
Nodes (4): Test snackbar notifications, Test snackbar when arrangement limit is reached, Test snackbar when clicking premium feature, TestSnackbarNotifications

### Community 138 - "TestProgressiveDisclosure"
Cohesion: 0.33
Nodes (4): Test progressive disclosure of features, Test that free users clearly see what they can do, Test that premium features are clearly marked, TestProgressiveDisclosure

### Community 139 - "TestAccessibility"
Cohesion: 0.33
Nodes (4): Test accessibility features of UI feedback, Test that color is not the only way to convey information, Test that icons supplement text messages, TestAccessibility

### Community 140 - "TestUsageTrackerPersistence"
Cohesion: 0.33
Nodes (4): Test data persistence, Test that usage data persists between tracker instances, Test that data survives save/load cycle, TestUsageTrackerPersistence

### Community 141 - "TestUploadStatusMessage"
Cohesion: 0.33
Nodes (4): Test upload status messages, Test that free users see status message about no upload, Test that guests see login required message, TestUploadStatusMessage

### Community 142 - "TestUploadButtonIcon"
Cohesion: 0.33
Nodes (4): Test upload button icon changes based on user, Test that free users see lock icon on upload button, Test that premium users see upload icon, TestUploadButtonIcon

### Community 143 - "TestUploadWorkflow"
Cohesion: 0.33
Nodes (4): Test complete upload workflow for different users, Test that free user cannot complete upload workflow, Test that premium user can complete upload workflow, TestUploadWorkflow

### Community 144 - "TestSaveStillWorks"
Cohesion: 0.33
Nodes (4): Test that save functionality still works for free users, Test that free users can still save videos locally, Test that save button is enabled for free users, TestSaveStillWorks

### Community 145 - "TestUIFeedback"
Cohesion: 0.33
Nodes (4): Test UI feedback for upload restrictions, Test that premium upsell banner shows for free users, Test that upload settings button is disabled for free users, TestUIFeedback

### Community 146 - "TestIntegrationUploadBlocking"
Cohesion: 0.33
Nodes (4): Integration tests for upload blocking feature, Test complete workflow of free user trying to upload, Test complete workflow of premium user successfully uploading, TestIntegrationUploadBlocking

### Community 147 - "TestPremiumFeatureMessaging"
Cohesion: 0.33
Nodes (4): Test messaging around premium features, Test that premium dialog mentions free users can still save, Test that premium features are accurately listed, TestPremiumFeatureMessaging

### Community 148 - "TestEdgeCases"
Cohesion: 0.33
Nodes (4): Test edge cases for upload blocking, Test that having a merged video doesn't bypass upload block, Test that upload button stays locked after save, TestEdgeCases

### Community 149 - "YouTube Data API v3"
Cohesion: 0.50
Nodes (4): FR-004 YouTube Upload (title, description, tags, privacy), YouTube API quota constraint (10,000 units/day), YouTube Data API v3, google-api-python-client==2.187.0

### Community 150 - ".test_build_youtube_service_with_valid_creds()"
Cohesion: 0.50
Nodes (3): Test YouTube API service building, Test building YouTube API service with valid credentials, TestYouTubeServiceBuilding

### Community 151 - ".test_get_user_info_from_credentials()"
Cohesion: 0.50
Nodes (3): Test user info retrieval from OAuth, Test retrieving user info from credentials, TestGetUserInfo

### Community 152 - "TestStepIndicatorForGuest"
Cohesion: 0.50
Nodes (3): Test step indicator shows correct state for guests, Test that step 2 indicator shows guest skip message, TestStepIndicatorForGuest

### Community 153 - "test_same_codec_preview()"
Cohesion: 0.50
Nodes (3): Test cache processor with same-codec videos (should be fast), Test preview generation with same-codec videos (H.264 only), test_same_codec_preview()

### Community 154 - "Flet 0.28.3 GUI framework"
Cohesion: 0.67
Nodes (3): Flet 0.28.3 GUI framework, flet==0.28.3, flet-video==0.1.1

## Ambiguous Edges - Review These
- `PurchasePlan` → `Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99)`  [AMBIGUOUS]
  docs/PREMIUM_PURCHASE_IMPLEMENTATION.md · relation: conceptually_related_to
- `FreeRole` → `Multi-Role System (Guest / Free / Premium / Admin)`  [AMBIGUOUS]
  README.md · relation: conceptually_related_to
- `AuditLogService` → `AuditLogViewer component (documented)`  [AMBIGUOUS]
  docs/AUDIT_LOG_VIEWER_IMPLEMENTATION.md · relation: conceptually_related_to
- `Multi-Role System (Guest / Free / Premium / Admin)` → `YouTube Upload Blocking for Free Users (premium upsell)`  [AMBIGUOUS]
  docs/NEW_FEATURES_TEST_SUMMARY.md · relation: conceptually_related_to
- `Multi-Role System (Guest / Free / Premium / Admin)` → `Firestore Data Model (users, audit_logs)`  [AMBIGUOUS]
  docs/VideoMergerandUploaderDocu.pdf · relation: conceptually_related_to
- `Multi-Role System (Guest / Free / Premium / Admin)` → `Python/Firebase Access Control Integration (Pyrebase FirebaseAuth / UserSession)`  [AMBIGUOUS]
  README.md · relation: conceptually_related_to
- `Premium Purchase System (mock, lifetime PHP 5.00)` → `Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99)`  [AMBIGUOUS]
  docs/PREMIUM_PURCHASE_IMPLEMENTATION.md · relation: conceptually_related_to
- `Defense in Depth Strategy (UI / Backend / Firebase rules / Audit / Rate limiting)` → `Recommended Firestore Security Rules (isAdmin, future web deployment)`  [AMBIGUOUS]
  docs/ADMIN_DASHBOARD_TODO.md · relation: conceptually_related_to
- `token.pickle OAuth token storage` → `NFR-003 Security (pickled tokens, no stored passwords)`  [AMBIGUOUS]
  README.md · relation: conceptually_related_to
- `Testing & Quality Assurance (pytest, claimed 100+ tests)` → `Core Test Suite (124 tests, 104 passing, 83.9%)`  [AMBIGUOUS]
  docs/TEST_SUMMARY.md · relation: conceptually_related_to
- `Free User Daily Arrangement Limit` → `New Features Test Suite (6 files, 245+ tests)`  [AMBIGUOUS]
  docs/NEW_FEATURES_TEST_SUMMARY.md · relation: conceptually_related_to
- `Free User Daily Arrangement Limit` → `User Capabilities Matrix (Guest / Free / Premium / Admin)`  [AMBIGUOUS]
  docs/VideoMergerandUploaderDocu.pdf · relation: conceptually_related_to
- `admin_audit_logs Firestore collection` → `Firestore Data Model (users, audit_logs)`  [AMBIGUOUS]
  docs/VideoMergerandUploaderDocu.pdf · relation: conceptually_related_to
- `User Capabilities Matrix (Guest / Free / Premium / Admin)` → `YouTube Upload Blocking for Free Users (premium upsell)`  [AMBIGUOUS]
  docs/VideoMergerandUploaderDocu.pdf · relation: conceptually_related_to

## Knowledge Gaps
- **18 isolated node(s):** `videomerger-app`, `videomerger_app_revamp (successor project)`, `flet==0.28.3`, `flet-video==0.1.1`, `ffmpeg-python==0.2.0` (+13 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 1077 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `PurchasePlan` and `Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `FreeRole` and `Multi-Role System (Guest / Free / Premium / Admin)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `AuditLogService` and `AuditLogViewer component (documented)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Multi-Role System (Guest / Free / Premium / Admin)` and `YouTube Upload Blocking for Free Users (premium upsell)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Multi-Role System (Guest / Free / Premium / Admin)` and `Firestore Data Model (users, audit_logs)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Multi-Role System (Guest / Free / Premium / Admin)` and `Python/Firebase Access Control Integration (Pyrebase FirebaseAuth / UserSession)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Premium Purchase System (mock, lifetime PHP 5.00)` and `Premium Plans (Monthly $9.99 / Yearly $99.99 / Lifetime $299.99)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._