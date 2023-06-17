# InedibleOS

**Install image password is "live" without the quote.**

# Build instructions

**Requirements (Build Environment):**\
Arch Linux REQUIRED as a build environment (Manjaro **DOES NOT WORK** even though it is based on Arch)\
Future arm64 support is planned.

**Device requirement:**\
PC/Mac with at least 8 GB of ram, 50 GB of free disk space and 2 cores of x86_64 CPU (Using virtual machine might require more resources).


**Building Process**
1. Go in opt/ezrepo, check the calamares-dependencies.txt for any required but not installed dependencies.
2. Open the terminal in opt/ezrepo, then copy and paste this command:
```
./build.sh
```
3. Open the terminal in the project's root folder, then execute these commands.
```
su
```
```
./clean.sh
```
```
./build.sh
```
4. The iso file will be created outside of the root folder.
