---
title: KB1 - Microphone Sleeps or Becomes Unresponsive Using OBS
description: The microphone may become unresponsive when using OBS
layout: default
---
<h1>KB1 - Microphone Sleeps or Becomes Unresponsive Using OBS</h1>

ISSUE: 

When using OBS the microphone may become unresponsive as the browser window is forced into the background

SOLUTION:

1. Running ZipCaptions as a Progressive Web App (PWA) will see the page running in its own browser instance. This will stop the microphone from sleeping. 

2. Adding https://zipcaptions.app to the [chrome://settings/performance page](chrome://settings/performance page ){:target="_blank"}{:rel="noopener noreferrer"} will prevent Chrome from putting the tab to sleep when you move away from it. 
