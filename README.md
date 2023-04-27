# InedibleOS

Don't make it public yet, I still need to check for license and stuff.

# Build instructions

**Requirements (Build Environment)**
1. Arch Linux REQUIRED in order to obtain the Arch Linux's kernel (except Manjaro **DOES NOT WORK** even though it is based on Arch)
2. Go in opt/ezrepo, check the calamares-dependencies.txt for any required but not installed dependencies.
3. Open the terminal in opt/ezrepo, then copy and paste this command:
```
./build.sh
```
4. Open the terminal in the project's root folder, then execute these commands.
```
su
```
```
./clean.sh
```
```
./build.sh
```
5. The iso file will be created outside of the root folder.
