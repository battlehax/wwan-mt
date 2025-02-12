# wwan-mt
wwan mpcie meshtastic interface for laptops
My dumb idea to make a Meshtastic node for the cellular modem slot on old Thinkpads and such.

# ideas
- Use a [mpcie2usb](https://www.amazon.com/Zer-one-Adapter-Converter-Expansion/dp/B07XD3Q2XM) with a tiny node, or design a complete board
- breakout usb lines from wwan slot [pinout](https://pinoutguide.com/Slots/mini_pcie_pinout.shtml)
- breakout battery, test voltages, current, while on/off/charging/full to apply [LDO](https://www.amazon.com/dp/B09WVBSKPY) [AMS1117](http://www.advanced-monolithic.com/pdf/ds1117.pdf)
- Sever usb +5v line, connect wwan-mt through an LDO or similar, directly to the laptop battery to keep node running at all times
- analyze internal 3g antennas with vna or find a suitable replacement
- investigate wake triggers with notification module
- rapid boot/resume, coreboot? tinycore?
