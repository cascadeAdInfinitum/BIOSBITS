# BIOSBITS
Compiled version of https://github.com/biosbits/bits
Use rufus dd image mode to make a bootable usb  
**NOT COMPATIBLE WITH RYZEN CPUS**

For AMD (AM4/AM5) compatible version, see [here](https://github.com/gamer043/bits-amd-smi-latency)  

If you want to compile it yourself (dont bother), use ubuntu 16.04.7 lts  
Make sure to change verbosity level to 3, so it shows exact smi count & latency values

# SMI Latency Test Results Table
| CPU  | MB | UEFI Version | Total Runs | SMI Count | SMI Latency | Image proof | Notes 
| ------------- | ------------- | ------------- | -------------|------------- | ------------- |-----------------|--------|
Thinkpad T430 | / | latest | 10 | 0 | 120 ns | / | Lowest value result thus far. Consistent.
R7 9850X3D | ASUS X870 Apex | ? | 10 | 897 | 68 µs | [link](https://i.imgur.com/CFkMYjt.png) | AMD-specific tool was used, results are here though.
i9-13900k | ASUS Strix Z790 D4 | ? | 0 | 5 | 75 µs | [link](https://i.imgur.com/IxKUi76.jpeg) | /
Xeon 2630V4 | Gigabyte X99-UD3 | F22 | 10 | 236 | 147 µs | / | Consistent latency value.
i7-8700k | ASUS Maximus X Apex (Z370) | 2.701 | 10 | 909 | 222–239 µs | [img](https://i.imgur.com/jv6DzmY.png) | Small variance
i7-3770k | Gigabyte Z77X-D3H | F14-F18 | 10 | 930 | 174–1400 µs | [link](https://i.imgur.com/vM1d5zr.jpeg) | The board isn't able to stabilize the results, keeps oscillating. Min & max were noted
i3-8100 | MSI Z370 SLI Plus | / | 10 | 909–915 | 1300–1400 µs | / | Consistent values
i7-13700k | MSI Z690 Unify X | ? | 10 | 0 | 10 ms | [link](https://i.imgur.com/nQtcgLR.png) |  z
