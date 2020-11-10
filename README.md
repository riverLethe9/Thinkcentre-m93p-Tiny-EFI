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

Everything works with the one exception of shutdown. It can sleep perfectly, but whenever I try shutting down, the display goes black but the LED indicators on the machine stay lit, and the fan is still spinning. I have investigated my USB port mapping to no avail. One thing I did notice is that the `pmset -g log` shows coreaudiod is very active when I am shutting down. 

