---
layout: post
title:  "Olauncher: The First Step to Minimalism"
date:   2026-02-14 12:00:00 +0500
categories: launchers minimalism
tags: olauncher customization adb
---

My journey to a minimalist Android experience started with the launcher. I needed something that wouldn't bombard me with icons and notifications the moment I unlocked my phone.

Enter **Olauncher**.

## Why Olauncher?

It's extremely lightweight, open-source, and text-based. No icons to distract you. Just a list of your most used apps.

## Key Features

*   **Text-only home screen:** Up to 8 apps.
*   **Daily wallpaper:** Automatic updates associated with the time of day.
*   **Gestures:** Swipe left/right to open apps or camera.

## Advanced Customization (ADB)

I used ADB to remove some bloatware that even Olauncher couldn't hide. Here is a useful command to list all installed packages if you are hunting down bloat:

```bash
adb shell pm list packages -f
```

And to uninstall a package for the user 0 (current user):

```bash
adb shell pm uninstall -k --user 0 com.example.bloatware
```

Use these commands with caution!
