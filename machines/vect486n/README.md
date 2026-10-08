# HP Vectra 486N (D26xxA)

- `f000-64k.rom`: supplied T.04.02 system BIOS, 08/27/92. This is only
  the 64 KiB F0000h block; the Setup/error-message modules are missing.
- `t0405-flash.rom`: complete 256 KiB HP T.04.05 flash image, 10/11/94.
- `c0202.rom`: complete 32 KiB HP Ultra VGA C.02.02 BIOS, 01/18/93.

The latter two files are extracted without modification from HP's updater:
https://ftp.hp.com/pub/softlib/software1/vc2007/vc2007en/t0405us.exe

Extract its ZIP member `RB0405US.BIN` (262160 bytes), then remove the 16-byte
header for `t0405-flash.rom`. The first 32768 bytes of that flash image are
`c0202.rom`. The system BIOS occupies its final 65536 bytes. These are original
HP firmware bytes; no cache bypass or other emulator patches are stored here.
The supplied 24 KiB C.01.00 VGA shadow dump is incomplete and is not included.

SHA-256:

```
105c1e45affea415ca19e54f8b8ca12e502d00cbb7002dddb781590f409d7f03  f000-64k.rom
72e659746507daf8e9d6c19f4a94b20a0dd13e45b398cd3f84f04ee84e3bccab  t0405-flash.rom
d8c16cc8611943a468a7484a628c5650f264495a957d158b8290f7e212ffbd01  c0202.rom
```
