# NAND Partition layout for the Broadmobi BM818

| Name     | Offset   | Length   | Attr          | Flash |
|----------|----------|----------|---------------|-------|
| sbl      | 00000000 | 00140000 | 0xff/0x1/0x0  | 0     |
| mibib    | 00140000 | 00140000 | 0xff/0x1/0xff | 0     |
| efs2     | 00280000 | 00600000 | 0xff/0x1/0xff | 0     |
| tz       | 00880000 | 00140000 | 0xff/0x1/0x0  | 0     |
| devcfg   | 009C0000 | 00060000 | 0xff/0x1/0x0  | 0     |
| info     | 00A20000 | 00060000 | 0xff/0x1/0x0  | 0     |
| mba      | 00A80000 | 00080000 | 0xff/0x1/0x0  | 0     |
| acdb     | 00B00000 | 00080000 | 0xff/0x1/0x0  | 0     |
| rpm      | 00B80000 | 00060000 | 0xff/0x1/0x0  | 0     |
| qdsp     | 00BE0000 | 02F40000 | 0xff/0x1/0x0  | 0     |
| apps     | 03B20000 | 00520000 | 0xff/0x1/0x0  | 0     |
| efs2bak  | 04040000 | 00300000 | 0xff/0x1/0x0  | 0     |
| firmware | 04340000 | 02F40000 | 0xff/0x1/0x0  | 0     |
| backup   | 07280000 | 00040000 | 0xff/0x1/0x0  | 0     |
| efs2apps | 072C0000 | 00D40000 | 0xff/0x1/0x0  | 0     |