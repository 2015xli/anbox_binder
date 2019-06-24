# Linux kernel module of binder/ashmem driver

This is the binder (and ashmem) driver module source package from anbox. It is already out of sync with current Linux kernel tree, but it is still useful in certain situations. 

To download the files for binder (and ashmem) module to a Linux box (that has no builtin binder driver):

    $ sudo add-apt-repository ppa:morphis/anbox-support
    $ sudo apt update
    $ sudo apt install anbox-modules-dkms

To install the driver modules:

    $ sudo modprobe ashmem_linux
    $ sudo modprobe binder_linux


To remove the kernel modules (and files) installed above:

    $ sudo apt install ppa-purge
    $ sudo ppa-purge ppa:morphis/anbox-support
