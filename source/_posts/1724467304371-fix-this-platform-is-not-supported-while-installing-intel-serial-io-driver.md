---
title: Fix “This Platform Is Not Supported.” While Installing Intel Serial IO Driver
date: 2024-08-25T15:32:50.733Z
updated: 2024-08-26T15:32:50.733Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: This Article Describes Fix “This Platform Is Not Supported.” While Installing Intel Serial IO Driver
excerpt: This Article Describes Fix “This Platform Is Not Supported.” While Installing Intel Serial IO Driver
thumbnail: https://thmb.techidaily.com/cb70e57700d07e1f21d91f89b112cf1e7299f5606065c397aa28c9965f8c1a6d.jpg
---

## Fix “This Platform Is Not Supported.” While Installing Intel Serial IO Driver

While installing Intel® Serial IO host controller driver, if you get error message **“The setup program ended prematurely because of the following error: This platform is not supported”** **,** don’t worry. The error can be easy to fix. The error would occur if I2C is not enabled in BIOS. To resolve the problem, just enable I2C in BIOS.

 [![1028](https://images.drivereasy.com/wp-content/uploads/2015/10/1028-300x244.png)](https://images.drivereasy.com/wp-content/uploads/2015/10/1028.png) 

  Please refer to the guide below how to enable I2C in BIOS.

  1\. Press **F2** during boot to enter BIOS Setup.

 2\. Go to the **Advanced** \> **Devices** \> **Onboard Devices** menu.

On the Legacy Device Configuration pane:

 3\. Set **Pins 13/14** to **I2C0\_SCL/I2C0\_SDA** .

 4\. Set **Pins 15/16** to **I2C1\_SCL/I2C1\_SDA** .

 5\. Press **F10** to save and exit BIOS Setup.

  After enabling I2C in BIOS, you can install the Intel® Serial IO host controller driver again.

 I2C is enabled for the Low Speed Custom Solutions Header. So if you don’t wish to use the Low Speed Custom Solutions Header, you don’t need to install this driver.

  If you use[Driver Easy](https://tools.techidaily.com/drivereasy/download/) to install this driver and meet this problem, follow the guide here and the problem will be resolved. Alternatively, you can skip to install this driver by clicking the arrow button and selecting**Hide this Update** .

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>



<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>



<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296740&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.nero.com/nero-com-wAssets/img/banners/2023/biu/Nero_BackItUp_Screen_2.webp" border="0"></a>
<!-- affiliate ads end -->