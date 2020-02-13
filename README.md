# VW-CEF
Chromium Embedded Framework (CEF) for VisualWorks.

See 
https://bitbucket.org/chromiumembedded/cef

Still at an very early stage. 

Based on
- CEF 3.3112.1659.gfef43e0 (2017-09-06)
- VisualWorks 8.1.1 / 8.3.2

Licensed under the MIT license (see Copyright)

# Quickstart

- Download Chromium, e.g. the matching Windows version: http://opensource.spotify.com/cefbuilds/cef_binary_3.3112.1657.g2c22842_windows64.tar.bz2
- Create a new directory (e.g. c:\cef)
- Copy all .dll/.bin files from the `Release` directory and all files from `Resources` to this directory
- Set this directory in the image: `LibChromium directory: 'c:\cef'`
- Open the browser with `CEF.BrowserUI open`

# Debugging

Chromium write debug messages to a file named `debug.log` (located in the VM directory)

## Linux
The Linux version is very unstable currently and crashes at startup a lot.

It is neccessary to put the following files from the CEF resources directory next to the VM (e.g. symlink):
```
icudtl.dat
natives_blob.bin
snapshot_blob.bin
```
## macOS
Currently not supported