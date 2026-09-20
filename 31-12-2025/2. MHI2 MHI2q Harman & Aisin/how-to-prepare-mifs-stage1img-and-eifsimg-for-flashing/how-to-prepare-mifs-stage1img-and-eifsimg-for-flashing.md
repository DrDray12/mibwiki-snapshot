# How to prepare mifs-stage1.img and eifs.img for flashing

:::warning
If on MHI2 you flash mifs-stage1.img or eifs.img without changing the header to ANDROID, MMX will stop booting and SD card access from RCC via /net/mmx/fs/sda0 will be lost. For recovery you'll need to flash NOR backup via [JTAG](https://mibwiki.one/doc/jtag-connection-to-rcc-or-mmx-o8C6JVpkZe) 😉

On [MHI2Q](https://mibwiki.one/doc/mhi2q-qualcomm-OjscS91N94) you don't need to do changes below!

:::

Open mifs-stage1.img in HxD, change AÿDÿOÿDÿ→ANDROID! and save the change.

 ![this mifs-stage1.img will brick the unit after flashing](attachments/10d49e0b-d8ab-4f2b-99a2-043bac2fa280.png)


 ![this mifs-stage1.img is correct!](attachments/1d3eb9d5-7673-4154-b7a4-a03fbcc05862.png)


\

\

\