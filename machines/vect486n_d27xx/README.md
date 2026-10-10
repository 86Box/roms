# HP Vectra 486N (D27xxA)

The extracted HP firmware is unmodified; the updater header is not included.

- `v0409-flash.rom`: complete 256 KB V.04.09 flash, system BIOS dated 04/11/95,
  including Setup D.04.03 and error-message modules.
- `vga10100.rom`: first 32 KB of the flash, HP Vectra 486 N & M VESA VGA BIOS
  version 1.01.00 for the integrated S3 86C805. Its 55 AA 40 header and byte
  checksum are valid.

The system block is the final 64 KB, with ID `HPD2751A`; its byte checksum is
also valid. The D27xxA firmware is distinct from the earlier D26xxA T-series.
V.04.04, V.04.07 and V.04.08 are documented but were not recovered.

SHA-256:

```
70e759b6a6a69c680f6be67e3dc8cc94eebb90b843de66c451f3adf5792c6167  v0409-flash.rom
b52dcbf4823ea3414fafb698836fdb98eb88dc4f7e83913ac3f1b764d5fa6806  vga10100.rom
```

References: [HP PC Service Handbook, Volume 2, chapter 13](https://manuals.plus/m/29dac22b29f9684e28eacf47d75918be4e263d8e039219d220f46d13e455b255.pdf),
[historical VBB1Z1US.EXE updater listing](https://www.cadstudio.cz/bbs-hw.htm).
