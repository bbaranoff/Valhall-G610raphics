# bifrost_opi5_patch
patch to make ability to compile kernel for orangepi5 with gpu bifrost enabled
apply the patch on
https://github.com/orangepi-xunlong/linux-orangepi/
```
git checkout orange-pi-5.10-rk3588
patch -p0 < bifrost.patch
cp config_tested .config
make menuconfig
make -j8
```
