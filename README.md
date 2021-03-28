```
Taking denilson-sá's answer further...

You need revision numbers to grab downloads. So first lookup the full version string from the following URL, adjusting parameters as needed:

https://omahaproxy.appspot.com/history.json?channel=stable&os=mac

For Chrome version 28 the full version string is 28.0.1500.71. Now go to https://omahaproxy.appspot.com and enter the full version string ("28.0.1500.71") into the Position Lookup box. Copy the Base Position number ("209842" in this case).

You can use that base position number and platform as a filter at either of these URLs:

http://commondatastorage.googleapis.com/chromium-browser-continuous/index.html
http://commondatastorage.googleapis.com/chromium-browser-snapshots/index.html
You probably won't have a perfect match on the base position number but you can at least use it to get close to the version you want.
```