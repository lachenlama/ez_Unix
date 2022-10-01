# ifconfig

**ifconfig**(interface configuration) command is used to configure the kernel-resident network interfaces. It is used at the boot time to set up the interfaces as necessary. After that, it is usually used when needed during debugging or when you need system tuning. Also, this command is used to assign the IP address and netmask to an interface or to enable or disable a given interface.

## Syntax:
``` bash
ifconfig [...OPTIONS] [INTERFACE]
```

Newer versions of some Linux distributions don’t have ifconfig command pre-installed. So, in case, there is an error “ifconfig: command not found”, Then execute the following command to install ifconfig.

### For Debian, Ubuntu, and related Linxu distributions
``` bash
sudo apt-get install net-tools
```

### For CentOS or RPM(RedHat Package Manager) based Linux
``` bash
yum install net-tools
```