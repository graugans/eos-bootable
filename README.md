# Create a bootable media for Canon DSLRs

This is based on the [Magic Lantern](https://www.magiclantern.fm/) source code. The purpose of this project is to 
provide me a backup for patching the CF card of my Canon 350D DSLR.


## Build Instructions

Follow these steps to build the project:

### Clone the repository

```sh
git clone https://github.com/graugans/eos-bootable.git
```

Navigate into the project directory and run CMake

```sh
cd eos-bootable
cmake -B build
cmake --build build
```

To use the file `make_bootable.sh` you have to copy the `exfat_sum` binary from the build folder to the project root.

```sh
cp build/exfat_sum .
```
