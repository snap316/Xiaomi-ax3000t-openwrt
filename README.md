Cloud compilation of OpenWrt firmware for Xiaomi AX3000T and flashing tutorial and flashing back official tutorial
The firmware can be customized by modifying the config file

Theoretically, it is possible to compile firmware for any supported model and any configuration

If you need to add some plugins that are not available by default in LEDE, you can modify the workflow file, that is, by modifying the cloud compilation workflow file to git the required plugin source code to compile these plugins (such as the new version of the argon theme and ddns-go)

Please do not use the browser's web page translation when looking at the README, as it will cause the layout of the README to be incorrect.

If you are using the firmware released in Releases, then there should be no strange problems such as not being able to flash and not being used, if you are using the firmware compiled by you modifying the configuration file yourself through the cloud, I can only ensure that the firmware can be compiled, and whether it can be flashed in and used normally is not guaranteed.

Instructions for flashing openwrt with uboot: uboot selects the third qwrt when flashing firmware on July 8 and earlier, uboot selects the second option when flashing firmware on August 4 and later, and when upgrading firmware from July 8 and before, please back up the configuration file in the backup/upgrade option first, and then go to uboot to upgrade, select the second option, and then upgrade againRestore the previous configuration file in a backup/upgrade.

See how to generate a config file
Other important parts
1. The default login IP is 192.168.1.1

2. The default login password is password

3. It cannot be used during cloud compilation, which will cause compilation failure!!ssh
