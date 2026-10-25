# fix-tablet update channel

The application reads `update.json` before showing the login window.

To require an update, change `version` to a value different from the app build constant (`AuthService.AppVersion`), then commit the change to `main`. The application will show the update window and will not open the login or main window.

Change `mediaFireUrl` and `websiteUrl` in the same file to change the buttons shown in the update window.

Keep this repository public because the application reads the raw file without a GitHub token.
