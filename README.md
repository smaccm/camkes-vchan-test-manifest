camkes-vchan-test-manifest
==========================

Testing ground for AADL to vchan communication.

The example without AADL-generated code

    make vchan_defconfig; make

The example with AADL-generated code

    make vchan_aadl_defconfig; make

Both should run on x86 with qemu

    qemu-system-i386 -nographic -m 512   -kernel images/kernel-ia32-pc99   -initrd images/capdl-loader-experimental-image-ia32-pc99

camkes-vm-manifest
==================
The CAmkES VMM is a Virtual Machine Monitor that utilizes the CAmkES component platform.
Due to the static nature of CAmkES systems the VMM is specified at build time to run
on a particular hardware platform. Currently the VMM is mostly targeted to run on the
C162 platform from Aitech. There is also a configuration for running on generic x86
machines, but it has almost no hardware support.

For general instructions on how to use this repository, see [sel4.systems](http://sel4.systems/Download/building).

For general information about CAmkES see [the CAmkES pages on seL4.systems](http://sel4.systems/CAmkES).

For detailed information about CAmkES see documentation in [the camkes-tool repo](https://github.com/seL4/camkes-tool/blob/master/docs/index.md).

For detailed information about the VM on the C162 platform see the doucmention in [the camkes-vm repo](https://github.com/seL4/camkes-vm/blob/master/README.md).
