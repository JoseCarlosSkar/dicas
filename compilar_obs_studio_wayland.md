```bash
$ sudo dnf copr enable sentry/v4l2loopback
$ sudo dnf install v4l2loopback-dkms

$ sudo dnf install cmake git ninja-build clang wayland-devel libcurl-devel zlib-devel mbedtls-devel speexdsp-devel
$ sudo dnf install libX11-devel mesa-libGL-devel libv4l-devel pulseaudio-libs-devel libXcomposite-devel luajit-devel swig pipewire-devel
$ sudo dnf install qt5-qtsvg-devel qt5-qtwayland-devel qt5-qtbase-private-devel qt5-qtbase-devel

$ sudo dnf -y install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
$ sudo dnf install ffmpeg-devel x264-devel libftl-devel

$ git clone --recursive https://github.com/GeorgesStavracas/obs-studio
$ cd obs-studio

$ mkdir build && cd build
$ cmake -DUNIX_STRUCTURE=1 -GNinja ..
$ ninja && sudo ninja install

$ sudo echo "/usr/local/lib" >> /etc/ld.so.conf.d/local.conf
$ sudo ldconfig
```
