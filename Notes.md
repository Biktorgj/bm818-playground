# Notes

1. You can jump to EDL mode by sending: `echo -ne "AT+BMCMD=EDL\r\n" > /dev/ttyUSB2`
2. Secure boot is *disabled*
```
Sec_Boot0 PKHash-Index:0 OEM_PKHash: False Auth_Enabled: False Use_Serial: False
Sec_Boot1 PKHash-Index:0 OEM_PKHash: False Auth_Enabled: False Use_Serial: False
Sec_Boot2 PKHash-Index:0 OEM_PKHash: False Auth_Enabled: False Use_Serial: False
Sec_Boot3 PKHash-Index:0 OEM_PKHash: False Auth_Enabled: False Use_Serial: False
Secure boot disabled.
```
3. At this point I could just wipe the entire flash and replace it with mine but it's probably not going to boot as is and I haven't yet found a USB_Boot testpoint to enter QDL mode directly
4. The loader in EDL_Loader/ can be used to peek memory and not only read the flash
