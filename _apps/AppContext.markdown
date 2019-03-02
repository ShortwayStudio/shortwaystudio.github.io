---
layout: app-page
title:  "AppContext"
description: "Better application context for Tasker with Xposed!"
backgroundColor: 03a9f4  # 03a8f5   10b4ee
textColor: ffffff
# icon: "res/apps/appcontext/icon.png"
lead: >
  Have Tasker react on running applications, without the downsides of the default implementation!
youtube_id: dmhjFhWrjsM
google_play_id: io.shortway.appcontext
xda_labs_id: io.shortway.appcontext
xposed_repo_id: io.shortway.appcontext
---
*[Requires Xposed and Tasker (or equivalent)]*
  
The default application context of Tasker has several downsides:
*  it is inaccurate (in Android versions after KitKat)
*  it needs an accessibility service, which prevents using screen lock to enhance data encryption
*  it checks frequently which app is running
Especially the last point is inconvenient, as frequent checks may drain battery and infrequent checks means Tasker is slow to react.
  
AppContext solves these problems by utilizing the power of Xposed! It hooks directly into the Activity-class, letting Tasker react immediately when an app starts. This means no more periodic checking which app is running, so no more battery drain and no more slow reactions. It's also perfectly accurate and doesn't need an accessibility service, so your device's screen lock can be used for enhanced data protection again.
(Experimental support for reacting on Services is also present.)
  
AppContext may also work with other apps using the Locale API, such as Locale, Llama, Automate, Automagic and others. However, this is not tested extensively.
  
To support development, AppContext contains non-intrusive ads. These can be removed with a small in-app purchase.
  
Please understand that AppContext is still considered to be in beta. There may be bugs.
  
##### CREDITS
*  Crafty Apps EU/Pent/João Dias for developing Tasker
*  rovo89 for creating the Xposed Framework
