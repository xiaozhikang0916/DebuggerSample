# DebuggerSample

A simple project to reproduce *Unable to find project context to attach debugger* issue of Android Studio after Iguana Canary 8.

[Google issue tracker](https://issuetracker.google.com/issues/307194650)

## To reproduce

Clone this project, then build and run. It is fine to attach a debugger to the process so far.

Then comment out the app module in `settings.gradle.kts#L23`, or switch to the `failure` branch, and sync, then `Error running 'Attach Debug to Process'` comes up if try to attach a debugger.
