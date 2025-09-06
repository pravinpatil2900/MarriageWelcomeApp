
# MarriageWelcomeApp

Android (Kotlin + Jetpack Compose) form app that sends a welcome message via Betablaster API on submit.

## Fields
- ID No
- Name
- Mobile Number (auto `91` prefix if missing)
- Staff Name
- Next Visit Date
- **Submit** button

## How to use with GitHub

1. Create a new GitHub repo (empty, no README/License initially).
2. Extract this project locally and run:

```bash
git init
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git add .
git commit -m "Initial commit: MarriageWelcomeApp"
git push -u origin main
```

3. GitHub Actions will start automatically and build the **release APK**.
   - Check **Actions** tab → latest workflow run.
   - Download artifact **app-release-apk** → `app-release.apk`.

## Local build (Android Studio)
- Open the project folder in Android Studio.
- Let Gradle sync, then **Build > Build APK(s)**.

## API credentials
Currently set in code (MainActivity.kt) as:
- `instance_id=6881CE8BC1285`
- `access_token=6881cc07a4e27`

Change URL if you need to update credentials.

> Tip: For security, prefer reading IDs/tokens from `local.properties` or GitHub Actions secrets and inject via `BuildConfig` in a future update.
