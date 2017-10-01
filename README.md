# VW-CEF
Chromium Embedded Framework (CEF) for VisualWorks.

See 
https://bitbucket.org/chromiumembedded/cef

Still at an very early stage. 

Based on CEF 3.3112.1659.gfef43e0 (2017-09-06)

Licensed under the MIT license (see Copyright)

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