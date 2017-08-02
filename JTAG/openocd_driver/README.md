How to use this driver for OpenOCD programm.
==========
Since with [this commit](http://openocd.zylin.com/gitweb?p=openocd.git;a=commitdiff;h=6b9d19d3675a82ccc501fd7cba036c5b04d04590) and [this fix](http://openocd.zylin.com/gitweb?p=openocd.git;a=commitdiff;h=1025be363e2bf42f1613083223a2322cc3a9bd4c) now OpenOCD program support SPI driver for ATH79 SoCs.

*This means, that you do NOT need to patch the OpenOCD program for support the ath79-spi driver. However, you may need to change the /openocd/src/flash/nor/spi.c source file for support your NOR-flash chip with specific JEDEC ID.*

**[Full description](https://wiki.openwrt.org/doc/recipes/debrick.ath79.using.jtag)** for parallel port build...
