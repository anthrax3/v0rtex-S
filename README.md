# v0rtex-S

A very basic App for testing Siguza's [v0rtex](https://github.com/Siguza/v0rtex) kernel exploit.

This fork also includes r/w access to / (aka disk0s1s1), on top of the previously given r/w access to /var.

Fat creds to stek on the r/w stuff, and originally xerub too. 

Added amfi patch. Thanks to: xerub && theninjaprawn. To see how to trust binaries see the comments in amfi.m. Doesn't support binaries located in /var or stashed binaries because sandbox isn't patched. \

Coming soon: loading tweaks via cycript & running SSH and Cydia if I have time. Will release a demo before that on my Twitter: @Jakeashacks
If you can't wait make a bootstrap.tar containing cycript & MobileSubstrate (cycript needs some binaries from the framework to work, also we need substrate to load all tweaks at the same time. Substrate iself does **NOT** work. See the code in amfi.m to get an idea how it works)

### Offsets

The offsets used are for iPhone 7 on iOS 10.3.1 and must be changed if that's not what you're using.

Offsets for iPod 6G (iPod7,1) 10.3.3, iPhone 7 (iPhone9,1) 10.3.3 and iPhone 6S (iPhone8,1) 10.3.2 are also included, however you will have to be a big boy and switch them out yourself in the v0rtex.m file.

To find your own offsets read [this guide](https://gist.github.com/uroboro/5b2b2b2aa1793132c4e91826ce844957).


### Requirements

Xcode and a device running iOS 10.3.x.
