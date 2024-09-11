# VMWare host modules fork

My fork of the [VMWare host modules](https://github.com/mkubecek/vmware-host-modules) repository, with some changes:

- updated the sources to the lastest Workstation Pro version
- applied the patches from the upstream repo, solving conflicts, and skipping the fixes that have been made upstream
- skipped @nan0desus' patches, since the issues have been solved upstream
- applied a patch to fix spurious network disconnections (originally from fluentreports.com, but considerably improved)
- added a small script to pack and install the patched modules

The master branch contains the latest Workstation version with the patches. For each patched version, there is a branch named `workstation-$vmware_version-sav`.

For reference, the tarballs with the source drivers are:

- `/usr/lib/vmware/modules/source/vmmon.tar`
- `/usr/lib/vmware/modules/source/vmnet.tar`
