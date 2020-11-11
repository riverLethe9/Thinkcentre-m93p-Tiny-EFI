# Thinkcentre-m93p-Tiny-EFI

**Processor**: i5 4570T

**GPU**: Intel 4600

**RAM**: 8GB

**SSD**: Samsung EVO 500GB

**Wifi/Bluetooth**: Azurewave BRCM94352HMB

**Audio**: ALC283 (layout 15)

**macOS version**: 10.15.7 (Catalina)

**Booter**: OpenCore 0.6.3

---

Everything works with the one exception of shutdown. It can sleep perfectly, but whenever I try shutting down, the display goes black but the LED indicators on the machine stay lit, and the fan is still spinning. 

One thing I did notice is that the `pmset -g log` shows coreaudiod is very active when I am shutting down. 

In the beginning, the machine would not sleep properly. USB mapping fixed that. But when sleep started working, shutdown stopped working. That leads me to think that I've done something wrong with the USB port mapping. I've tinkered around with it for a few months, but nothing has made a difference.

I tried the opencore FixShutdown ssdt and patch combo. That did not work.

I've tried changing SMBIOS to MacMini but that also did not do anything.

I tested for RTC issues, but there do not appear to be any bad regions. 

CFG-Lock is not present in my BIOS settings. VerifyMsrE2.efi tells me that my CFG is locked, but the system boots perfectly. I tried using the (alternative method)[https://www.reddit.com/r/hackintosh/comments/hz2rtm/cfg_lockunlocking_alternative_method/] with the RU.efi tool, but CPUSetup does not show up in the list.

