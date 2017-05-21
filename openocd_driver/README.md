How to use this driver for OpenOCD programm.
==========
**[Full description](https://wiki.openwrt.org/doc/recipes/debrick.ath79.using.jtag)** for parallel port build.

Keep in mind, **JEDEC ID** of flash memory is located in **<git or svn clone DIR>**/src/flash/nor/spi.c - and you may need to change it for your needs.

After configure the OpenOCD for your JTAG dongle, you just need to patch the program, and then make the programm via command:
```
git apply -3 < f891808.diff
make
sudo make install
```

Or you can use patch util:
```
patch -u -p1 < f891808.diff
make
sudo make install
```
*Where **patchfile.patch** must be placed in the trunk or other branches directory.*
