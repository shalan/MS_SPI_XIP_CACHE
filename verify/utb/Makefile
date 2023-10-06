SIM-RTL:
	iverilog MS_SPI_XIP_CACHE_ahbl_tb.v ../../hdl/rtl/MS_SPI_XIP_CACHE.v ../../hdl/rtl/bus_wrappers/MS_SPI_XIP_CACHE_ahbl.v ./vip/sst26wf080b.v
	./a.out

SIM-GL-16:
	iverilog -s MS_SPI_XIP_CACHE_ahbl_tb MS_SPI_XIP_CACHE_ahbl_tb.v ./vip/sst26wf080b.v ../../hdl/gl/sky130/16x16/MS_SPI_XIP_CACHE_ahbl.v ../../util/tech/sky130/sky130_hd.v
	./a.out

SIM-GL-32:
	iverilog -s MS_SPI_XIP_CACHE_ahbl_tb MS_SPI_XIP_CACHE_ahbl_tb.v ./vip/sst26wf080b.v ../../hdl/gl/sky130/32x16/MS_SPI_XIP_CACHE_ahbl.v ../../util/tech/sky130/sky130_hd.v
	./a.out
