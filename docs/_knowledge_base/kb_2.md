---
title: KB2 - Microphone Volume is Automatically Adjusted
description: The volume of the microphone is adjusted automatically by Zip Captions
layout: default
---
<h1>KB2 - Microphone Volume is Automatically Adjusted</h1>

ISSUE: 

When using Zip Captions in Chrome on Windows, the volume of the microphone is adjusted, and in a recording the user cannot be heard.

CAUSE:

Chrome has the ability to manage the volume of the microphone. This setting is called "WebRTC adjust the input volume".

SOLUTION:

1. Disable the feature by turning off the following Chrome Flag: 'WebRTC to adjust the input volume'. In order to do this, go to [chrome://flags](chrome://flags){:target="_blank"}{:rel="noopener noreferrer"} and search for the 'WebRTC to adjust the input volume' flag. Turn it off by changing the drop down to 'Disabled'.

2. Installing the 'Disabled Automatic Gain Control' Google Chrome Extension from the Chrome Web Store will also disable this feature. You can find it at [https://chromewebstore.google.com/detail/disable-automatic-gain-co/clpapnmmlmecieknddelobgikompchkk?pli=1](https://chromewebstore.google.com/detail/disable-automatic-gain-co/clpapnmmlmecieknddelobgikompchkk?pli=1){:target="_blank"}{:rel="noopener noreferrer"}.