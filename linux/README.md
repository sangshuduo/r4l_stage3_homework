# Linux kernel 6.1.12+1

Upgrade to Linux kernel 6.1.12+1

### Compilation

Requires dependent libraries

```
apt install gcc-aarch64-linux-gnu g++-aarch64-linux-gnu

apt install libelf-dev libgmp-dev libmpc-dev
```
Compile kernel image

```
make CROSS_COMPILE=aarch64-linux-gnu- ARCH=arm64 O=build bsta1000b_defconfig

make CROSS_COMPILE=aarch64-linux-gnu- ARCH=arm64 O=build -j8

make CROSS_COMPILE=aarch64-linux-gnu- ARCH=arm64 O=build modules -j8
```
