This is just a set of scripts to rebuild a known working kernel for ARM devices.

Script Bugs: "bugs@rcn-ee.com"

Step 1: Clone repo

```
git clone https://github.com/RobertCNelson/yakbuild
cd ./yakbuild/
```

Step 2: create recipe.sh

```
cp recipe.sh.sample recipe.sh
```

Step 3: edit recipe.sh

Step 3a: Enable toolchain:

```
#toolchain="gcc_linaro_eabi_4_8"
#toolchain="gcc_linaro_eabi_4_9"
#toolchain="gcc_linaro_eabi_5"
#toolchain="gcc_linaro_eabi_6"
#toolchain="gcc_linaro_eabi_7"
#toolchain="gcc_arm_eabi_8"
#toolchain="gcc_arm_eabi_9"
#toolchain="gcc_linaro_gnueabihf_4_7"
#toolchain="gcc_linaro_gnueabihf_4_8"
#toolchain="gcc_linaro_gnueabihf_4_9"
#toolchain="gcc_linaro_gnueabihf_5"
#toolchain="gcc_linaro_gnueabihf_6"
#toolchain="gcc_linaro_gnueabihf_7"
#toolchain="gcc_arm_gnueabihf_8"
#toolchain="gcc_arm_gnueabihf_9"
```

Step 3b: Enable choosen kernel_tag (uname -r)

```
kernel_tag="4.14.108-ti-r127"
```

Step 4: build

```
./build_kernel.sh
```
