# MS_SSPI_XIP_CACHE
SPI Flash memory controller with the following features:
- AHB lite interface
- Execute in Place (XiP)
- Nx16 Direct-Mapped Cache (default: N=32).

Intended to be used with SoCs that have no on-chip flash memory. 

## Todo:
 - [ ] support for WB bus
 - [ ] Support cache configurations other than 16 bytes per line

## Performance
The following data is obtained using Sky130 HD library
### Timing
- SCK to system clk ration : 0.5
- Hit Time : 1 cycle
- Miss Penality : 320 cycles (line size = 16 bytes)
### Power
| Configuration | # of Cells (K) | Delay (ns) | I<sub>dyn</sub> (mA/MHz) | I<sub>s</sub> (nA) | 
|---------------|----------------|------------|--------------------------|--------------------|
| 16x16 | 7.4 | 11.8 | 0.0625 | 20 |
| 32x16 | 14.3 | 17  | 0.126 | 39.5 |

