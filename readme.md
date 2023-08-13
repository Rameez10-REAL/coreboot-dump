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

Do "diff build/t430_coreboot_seabios_aa1efece74_top.rom ~/files/custom-coreboot-img/coreboot/prebuilt/skulls-1.0.8/t430_coreboot_seabios_free_aa1efece74_top.rom"

If they are no diffrence between stock compiled and prebuilt. You are doing everything right.

Now make sure you image maches the coreboot spashboot/spashscreen specifations and do du to make sure it the same size as stock 


[user@desktop ~/files/custom-coreboot-img/coreboot/compiledandcustom/skulls/t430]$ du bootsplash.jpeg 
16	bootsplash.jpeg
[user@desktop ~/files/custom-coreboot-img/coreboot/compiledandcustom/skulls/t430]$ du bootsplash1.jpg 
16	bootsplash1.jpg

It has to be a 1024x768 jpg with 


    "Progressive" turned off, and
    "4:2:0 (chroma quartered)" Subsampling




