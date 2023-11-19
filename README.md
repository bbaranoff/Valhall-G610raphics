```bash
clone repo...
cd
git clone https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git
cd linux
curl -o .bundle https://xff.cz/kernels/git/orange-pi-active.bundle
git fetch .bundle '+refs/heads/*:refs/remotes/megi/*'
git checkout orangepi5-6.6??
mv ../myrepocloned/linux.config .config
make menuconfig
make -j$(nproc)
sudo make install
sudo make headers_install
sudo make modules_install
sudo make dtbs_install
cd /boot
ln -s dtbs/6.6.0+ dtb
git clone https://github.com/JeffyCN/mirrors --branch libmali --single-branch
sudo aot install dolphin-emu
glxinfo -B (no HW acceleration ?????? :((((((( )
```

May have to check to thoses resources

- https://developer.arm.com/downloads/-/mali-drivers/valhall-kernel  
- https://armbian.site-meganet.com/dl/orangepi5-plus/archive/Armbian_23.8.99_Orangepi5-plus_jammy_edge_6.6.1_minimal.img.xz (fresh just found at writing time)  
- https://mega.nz/folder/j9QSDQSQ#6WpasOlbZYIInfw6yo4phQ/folder/LkgF1SoY  
- https://github.com/JeffyCN/mirrors/tree/libmali  
- https://github.com/Saikatsaha1996/mesa-Panfrost-G610  

