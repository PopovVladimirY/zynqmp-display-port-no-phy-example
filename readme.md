# ZynqMP standalone BSP customization for DP without PHY.

This project is a cusomisation of **cortexa53_0** platform libraries to adapt DPPSU and AVBUF to work wihtout PHY connected to DP source controller. It is based on v2019.2.01 VITIS SDK.

## How to use this project

This code shall replace content of the **(platform_top_cofiguration)/cortexa53_0** folder. 

>IMPORTANT: Build the platform project first, before replacing the content of the coretexa53_0 forlder. This is because during the first build of the platform project Vitis will copy the content of Xilinx SDK to it and will erase the updated files.

It shall be used in combination with user application adapted for the case. For instance, DP standalone example application implementing DP live video to PL to LCD scenario:

    https://github.com/PopovVladimirY/zynqmp-live-video-to-pl-no-phy-example.git

See the example application readme for details on project setup and use.