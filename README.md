# usingskia

I tried to build with SKIA using the tutorial https://skia.org/user/sample/building.

Repositories used in the wiki:<br>
SKIA: https://skia.googlesource.com/skia/<br>
GYP: https://chromium.googlesource.com/external/gyp.git<br>

Following are some of the things I did differently:

<b>SKIA Revision in DEPS:</b> Being lazy, I did not take the trouble of looking for the skia revision mentioned in the wiki. Instead I simply took the latest commit.<br>
<b>SKIA URL:</b> Though the wiki mentions "http" for the SKIA repo URL, I was getting an "SSL Required" error while running "gclient sync". Changing to "https" fixed this.<br>
<b>GYP URL:</b> I didn't use the var "googlesource_url" in my DEPS. Instead googled for the GYP repo which I found to be the one mentioned above and used that.<br>
<b>find_mac_sdk.py:</b> Instead of fetching this through DEPS, just installing Xcode seemed to do the job.<br>
