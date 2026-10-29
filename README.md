# MS Editor Media Hub — Native Android starter

This is a native Jetpack Compose Android project (not a WebView wrapper).

## Verified website categories
- Home
- Video Songs
- Video Tutorial
- Video Prompt
- Image Prompt
- Presets & Assets

These are the six categories requested for this native app. The category identifiers for the existing Supabase records must still be verified against the live website/database before connecting live media.

Website source verified from:
https://github.com/sajawalkhan12/ms-editor-media-hub-/blob/main/index.html

## Backend safety
- Existing Supabase project URL is configured in `app/src/main/java/com/mseditor/mediahub/SupabaseConfig.kt`.
- The website currently uses a public `sb_publishable_...` key. A publishable key is not a service-role key, but this project intentionally leaves it as a placeholder for you to paste from the existing website after confirming the current configuration.
- NEVER add a `service_role` or `sb_secret_` key to this app or GitHub.
- No database tables or storage buckets are created, modified, or deleted by this starter.

## Important
This is the initial native project scaffold. The verified website source shows the category names and Supabase URL/key, but exact live table column definitions, branding-settings storage paths, and the actual admin authorization policy still need checking before safely enabling uploads/deletes and shared engagement. Do not treat upload/delete as production-ready until those are verified.

## Build
Open the project in Android Studio on a computer, or use a compatible cloud Android build environment. GitHub mobile upload alone does not build an APK. See `BUILD_STEPS_ROMAN_URDU.md`.


## Launcher icon
The project now includes an emerald-green and gold MS launcher icon as native Android adaptive-icon resources. Android displays it as the app icon after a successful build/install.


## Original user-provided logo
The provided MS Editor Media Hub logo image is included at `app/src/main/assets/ms_editor_media_hub_logo.png` and used for the launcher icon in Android mipmap resources (`ic_launcher.png` and `ic_launcher_round.png`).
