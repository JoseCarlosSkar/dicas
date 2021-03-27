```bash
$ git clone --recursive https://github.com/GeorgesStavracas/obs-studio
$ cd obs-studio
$ git checkout gbsneto/pipewire

$ mkdir build && cd build
$ cmake -DUNIX_STRUCTURE=1 -GNinja ..
$ ninja && sudo ninja install

$ sudo echo "/usr/local/lib" >> /etc/ld.so.conf.d/local.conf
$ sudo ldconfig
```
