# InedibleOS

**Don't make it public yet, I still need to check for license and stuff.**

**Install image password is "live" without the quote.**

# Build instructions

**Requirements (Build Environment):**

Arch Linux REQUIRED as a kernel build environment (Manjaro **DOES NOT WORK** even though it is based on Arch)

Device requirement:

PC/Mac with at least 8 GB of ram, 50 GB of free disk space and 2 cores of x86_64 CPU (Using virtual machine might require more resources).


**Building Process**
1. Compile the kernel
```
makepkg -s
makepkg --skippgpcheck
```
2. Put the kernel package in opt/ezrepo
3. Put the output kernel file (vmlinuz-inKernel, initramfs-inKernel.img, initramfs-inKernel-fallback.img) in the root folder (will be generated when you build the OS inside work/x86_64/airootfs, just make sure you copy it before the build command delete it, you can leave the kernel file in the root folder as long as you do not update your kernel, or you will need to do it again with the new kernel.)
4. Go in opt/ezrepo, check the calamares-dependencies.txt for any required but not installed dependencies.
5. Open the terminal in opt/ezrepo, then copy and paste this command:
```
./build.sh
```
6. Open the terminal in the project's root folder, then execute these commands.
```
su
```
```
./clean.sh
```
```
./build.sh
```
7. The iso file will be created outside of the root folder.
