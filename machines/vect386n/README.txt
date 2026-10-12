HP Vectra 386N (D24xx)

Split from the original 128 KiB HP_Vectra_386-20_D2480_BIOS.BIN dump
supplied as hp-vectra-386-20-d2480-bios.zip. No bytes patched or omitted.
Original SHA-256: aef14e510169d8b621ae58ff4878c15e060af121f5f30fe8410904b5ad3f2678

vga.bin (32 KiB, original offsets 00000-07fff)
  HP/Video Seven Super VGA firmware, mapped at C0000 and E0000.
  SHA-256: 0301d5429cd85075e1dfaebd3d2c88631286d836091491da9acdebd45ec8a9a4

l0305.bin (96 KiB, original offsets 08000-1ffff)
  First 32 KiB: resident F2 setup at E8000, also accessed via the upper ROM alias.
  Last 64 KiB: system BIOS L.03.05, 08/09/91, mapped at F0000.
  SHA-256: e10d9c019870334ee9a3c66bec6ca7e7a66c93c1b6aa6080f7c89fd53a82d01e

Concatenating vga.bin followed by l0305.bin reproduces the original dump.
