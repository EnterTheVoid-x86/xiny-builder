# xiny-builder
Build toolchain for X.I.N.Y Linux

# What?
This is the placeholder repository for when I eventually upload the X.I.N.Y build toolchain.

# Why?
Easier to plan ahead.

# Who?
Refer to EnterTheVoid-x86/xiny.

# When?
Source will be published sometime in Late 2026.

# Okay, but what exactly is the plan?
X.I.N.Y uses top-of-the-tree software, a chroot for the squashfs, and a few commands to generate ISOs for building.

The plan? Automate this with a bash script and a few neat options :)

Eventually I want X.I.N.Y to be able to reproduce a build of itself, but this is far out of reach at the moment. Maybe you can help once source code is cleaned up and polished...

# Planned Design Documents?
- xiny-builder
  - Makefile
  - scripts
    - 1-git_repos.sh
    - 2-dependency_installer.sh
    - 3-configure_build_toolchain.sh
    - 4-generate_chroot.sh
    - 5-build_all_software.sh
    - 6-squashfs_dracut.sh
    - 7-generate_iso.sh
  - software
    - linux
    - coreutils
    - openrc
    - sysvinit
    - sed
    - nano
    - etc...
  - output
    - xiny.iso
    - bzImage
    - dracut.img
    - rootfs.sfs

This is the eventual layout I would like to have implemented.
