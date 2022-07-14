# NAND Partition layout for the Broadmobi BM818

| Name     | Description |
|----------|-------------|
| sbl      | Secondary boot loader |
| mibib    | Partition table |
| efs2     | Qualcomm EFS partition (where baseband params are stored) |
| tz       | TrustZone kernel |
| devcfg   | Unknown (*1) |
| info     | Empty |
| mba      | Presumably mba blob for the ADSP |
| acdb     | Audio calibration profiles (like *.acdb in linux based qcoms) |
| rpm      | Resource and Power Management firmware |
| qdsp     | Presumably modem blob for the adsp (modem.mdt) |
| apps     | Main OS |
| efs2bak  | Not the same as efs2, but similar content |
| firmware | Empty |
| backup   | Header: BroadMobi_RFNV, then empty |
| efs2apps | Unknown |

[1]
binwalk devcfg.bin 

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             ELF, 32-bit LSB executable, ARM, version 1 (GNU/Linux)
4520          0x11A8          Certificate in DER format (x509 v3), header length: 4, sequence length: 1135
5659          0x161B          Certificate in DER format (x509 v3), header length: 4, sequence length: 1030
6693          0x1A25          Certificate in DER format (x509 v3), header length: 4, sequence length: 1055
27598         0x6BCE          Linux kernel version 3.14.2
33312         0x8220          Unix path: /dev/buses/i2c_1

"Linux version 3.14.26-g43b1178-00038-g96ef344 (lnxbuild@abait242-sd-lnx) (gcc version 4.9.x-google 20140827 (prerelease) (GCC) ) #1 SMP PREEMPT Fri Jun 5 15:15:57 PDT 2015"
