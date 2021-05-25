# Log-Me-In

This UiPath Background process will monitor your Chrome browser to check for tabs where you were automatically signed out of the UiPath Cloud.

When this happens, it will sign you back automatically assuming that you are using a Microsoft account and that you are already signed into that account.

The first time it runs, it will not choose an Organization automatically. Instead, it will wait for you to click on it and remember your choice. Subsequent runs will pick that same organization.

The process has an input argument - "Reset". If set to true, the pre-selected organization will be forgotten, and the process will wait for you to choose another one.

To set it up:

1. Open this project in UiPath Studio
2. Publish to your personal workspace
3. Log in to Orchestrator and go to: My Workspace > Automations > Processes > Log.Me.In Process > More Options > Edit > Additional Settings
And check "Automatically Start Process

Now you can go in UiPath Assistant and run the process. It should run in the background on your machine and start automatically the next time you log in to your machine.

Another prerequisite is that, in the UiPath installer, you set UiPath Assistant op open when you log in to your machine.
