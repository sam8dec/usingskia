# usingskia

I tried to build with SKIA using the tutorial https://skia.org/user/sample/building.

Repositories used in the wiki:
SKIA: https://skia.googlesource.com/skia/
GYP: https://chromium.googlesource.com/external/gyp.git

Following are some of the things I did differently:

-SKIA Revision in DEPS: Being lazy, I did not take the trouble of looking for the skia revision mentioned in the wiki. Instead I simply took the latest commit.
-SKIA URL: Though the wiki mentions "http" for the SKIA repo URL, I was getting an "SSL Required" error while running "gclient sync". Changing to "https" fixed this.
-GYP URL: I didn't use the var "googlesource_url" in my DEPS. Instead googled for the GYP repo which I found to be the one mentioned above and used that.
-find_mac_sdk.py: Instead of fetching this through DEPS, just installing Xcode seemed to do the job.
