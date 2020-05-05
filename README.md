# modbuild
Kconfig project for Compile/Cross_Compile kernel module in a simple way

# Introduction
With this project you'll be able to Compile or Cross_Compile a kernel module.
Just simple type "make menuconfig" and configure module build

# Build Targets
	
    'menuconfig              -  Configure the module build'
    'gconfig                 -  Configure the module build with gtk interface'
	'savedefconfig           -  Save current config in a file called defconfig '
	'store           	 -  Save current config in configs directory with preferred name '
	'distclean               -  Clean all '
	'all                     -  Build the module'
	'install                 -  Install the module to your target'
	'flush                   -  Clean the module build'

Every target perform some action based on .config generated with menuconfig

# Makefile Variables

    MOD_NAME                -   Name of the module to build
    MOD_OBJS                -   Object used for module build
    KERNEL_DIR              -   Top directory of the kernel
    MOD_PATH                -   The path where the module source code is located
    INSTALL_DIR             -   The Directory where the module will be installed
    REMOTE_USR              -   User for SSH Connetion with remote target in case of Network Install
    REMOTE_PSW              -   Password of the SSH user in case of Network Install
    REMOTE_IP               -   IP of the remote Target in case of Network Install

    
