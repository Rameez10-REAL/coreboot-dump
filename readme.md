MD5 hash for the bineries

build/customsplash/t430.rom - f06d1331d7e390fb20e8c27e33b1ecda
Stock/prebuilt t430.rom (from https://github.com/merge/skulls/releases/download/1.0.8/skulls-1.0.8.tar.xz) - 81fd413fe8ca8bea80bc0bd0e39a50c3

TLDR the splash screen was replaced. This leads to the hashes being diffrent.
The hashes in my built one with "sudo ./build.sh" and docker match the prebuilt bineries. So it is compiling right.

	** WARNING **
coreboot has been built without an Intel Firmware Descriptor.
Never write a complete coreboot.rom without an IFD to your
board's flash chip! You can use flashrom's IFD or layout
parameters to flash only to the BIOS region.

4+0 records in
4+0 records out
4194304 bytes (4.2 MB, 4.0 MiB) copied, 0.00302839 s, 1.4 GB/s
==================== result: ======================
/home/coreboot/cb_build/t430_coreboot_seabios_aa1efece74_top.rom #This is coreboot/t430/build
===================================================
[user@computer ~/files/custom-coreboot-img/coreboot/compileda[user@computer ~/files/custom-coreboot-img/coreboot/compiledandcustom/skulls/t430]$ 

