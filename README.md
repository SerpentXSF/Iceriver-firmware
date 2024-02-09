# Iceriver-firmware
Iceriver KS Series Firmware - Original Creator Tswift and contributors - Join TeleGram https://t.me/swift_mining/3133

INSTRUCTIONS (this is ***VERY*** important):

1. We are obviously not liable for any potential damage to your hardware or loss of profits as a result

2. You acquire and use this firmware at your own risk

3. You thoroughly go over my recommendations for using this firmware which will be detailed below. PROOF OF HAVING THE COPPER HEATSINKS IS REQUIRED. YOU MUST SEND A PICTURE OF THE COPPER HEATSINKS INSTALLED ON THE MOSFETS NEXT TO THE MAC ADDRESS STICKER BEFORE RECEIVING THE FIRMWARE

4. You acknowledge that the 280 GH firmware is a safe and stable solution, and the use of 300+ firmware is not recommended if you are happy with your current results.

5. We are not responsible for any potential chip degradation from overclocking to 300+ GH

Warnings for KS0/KS0 Pro Overclocking

1. The cooling of the internal MOSFETs on the control board (circled in the attached picture) is the most important part of running 300+ GH firmware safely.  It is **REQUIRED** that the user applies 6x6x5mm (or very similarly sized) copper heatsinks to these 4 MOSFETs using non-conductive thermal glue to help dissipate the heat from them as they are not attached to the primary heatsink of the KS0 Pro chassis. Here are links to the heatsinks and thermal glue we recommend from US Amazon:

Be careful not to spread the thermal glue onto adjacent components and give the glue enough time to cure so that the heatsinks do not move when in use.

2. Airflow through the middle interior portion of the machine and to the heatsink is extremely important for 300+ GH overclocking. USB fans will not be sufficient (this is your warning). You need to use Axial fans (or stronger) or one of the specialized kits that is sold in the Telegram linked at the top of this Readme. Simply being in a cold ambient temperature environment is not enough. There needs to be focused, directed strong airflow; not just a high CFM fan blowing in the direction of the miner and having 90% of the air missing where you want it to go (inside the middle part of the machine). Just like before, you want to have a 120mm fan attached to the heatsink and blowing air TOWARD the heatsink (not away), and you want strong, focused airflow going through the middle internal section from the side with the power connection, not from the side with the Ethernet connection.

3.  It is strongly recommended that you replace the Thermal Paste on the chips and the Thermal Pads. We recommend using Arctic MX-6 Thermal Paste and Arctic TP-3 1.5mm Thermal Pads. US Amazon links:

AC Infinity Axial Fans kit with controller:
https://amzn.to/3vmrBUy

MOSFET heatsinks small:
https://amzn.to/3UdQ4Wp

MOSFET heatsinks Big:
https://amzn.to/3OfNmvV

Thermal Paste and Pads:
https://amzn.to/3u4WvR4
https://amzn.to/3u4WAnQ

4. To help with focusing and directing the airflow, we have a free 3D-printed side bracket that customers can have printed in their local area or online. The download link for the STL file to print is here: https://fastupload.io/SpCIiT76cOF7gWj/file - it is STRONGLY recommended that you do not attempt 300+ firmware without some sort of way to focus the airflow into the middle internal part of the machine.

5.  A 230w power supply is required for 340 GH. The increase in heat produced by the chips going from 320 GH to 340 GH is very significant. Expect the jump in temp to be anywhere from 10-20C difference. Do not underestimate this and do not run temps higher than 65-70C max.

6.  If you do attempt to use 300 GH or higher firmware, please start with 300 GH first and go up incrementally once you determine that everything is stable. If you have a "good" cooling solution, we would personally recommend not going past 300-320 GH. Only people with enthusiasts and excellent cooling solutions should attempt 340 GH. Once again, we recommend that people stick to 280 GH if they are happy with the results or if you are unsure of your cooling situation. Do not attempt the enthusiast upgrade if you are unsure of the potential to gain 20-60 GH. Only attempt this if you have read this entire guide and are confident in your cooling setup. 

To update a KS0/KS0Pro/KS1:
1. Unzip the file package
2. Reset the machine to factory settings, then restart
3. Upload the "INIT" file into the firmware upgrade, then restart
4. Upload the overclock file into firmware upgrade, then restart
5. Wait for the website interface to load, apply your pool settings, restart one more time and it will work after that

To update a KS2/KS3L/KS3M/KS3:
1. Unzip the file package
2. Reset the machine to factory settings, then restart
3. Upload the overclock file into firmware upgrade, then restart
4. Wait for the website interface to load, apply your pool settings, restart one more time and it will work after that

*Please also follow the readme notes included in the folder very carefully*

This firmware does NOT support SSL connections, make sure your pool connections are TCP. Our dev fee firmware is also not currently compatible with the HeroMiners pool. We are looking into fixing this. For now, please use a different pool: We recommend K1pool or Humpool.

Additional notes for KS0 Pro and KS3L/KS3M firmware:

KS0 Pro: https://t.me/swift_mining/1272
KS3L/KS3M: https://t.me/swift_mining/2308

It is also strongly recommended that you monitor the health of your ICERIVER miners and their chips using our free monitoring tool. This monitoring tool can help you spot overheating or overvolted chips and potentially save your miner from being damaged before it happens. The tool can be found here: https://t.me/swift_mining/2441

KS0 Instructions

1. Restore the miner to factory settings in the web interface or by pressing and holding the reset button. Allow the miner to restart
2. Upload the "INIT" file into the firmware upgrade menu and restart again
3. Upload the firmware with your desired overclock setting, then restart again
4. Apply your pool settings, set the fan speed to 100%, and observe hashrate. You can later decrease fan speed until you notice hashrate decrease
Use the following sequence: 340G_L, =>340G, =>320G_L, =>320G, =>300G_L, =>300G
If the hashrate does not meet expectations, try using a different firmware version in the third step.
When using this firmware, make sure your power supply is 180w or greater, and an external fan is installed blowing air TOWARDS the heatsink. AC-powered fans are much more effective than USB fans.

第一步，重置你的机器，恢复出厂设置
第二步，升级 INIT 固件，并且重启
第三步，升级有算力标志的固件，然后重启，之后修改你的矿池地址和钱包，并将内置风扇开到100%，然后观察算力。
使用顺序340G_L, =>340G, =>320G_L, =>320G, =>300G_L, =>300G
如果算力不符合预期，请在第三步中更换其他版本的固件。

使用这份固件，请确保你的电源在180W及以上，并且加装了外置风扇。

请拆开机器有网线接口和电源接口的面板，一共两块面板，使得空气可以在机器内部穿过，增加散热能力

如果有条件的话最好还是使用3D打印件+侧吹风扇。

额外增加的散热风扇如果不加装3D打印支架，请放置在机器的长散热鳍片一侧，往散热鳍片内吹风，最好使用2000转左右的风扇全速运行。


严重警告！！！此固件进行了设备唯一ID校验，如果将此固件烧写到非法设备上，造成的一切损失由自己承担！！我们概不负责！！！
Serious warning! This firmware performs device-unique ID verification, if you burn this firmware to an illegal device, you will be responsible for all damages caused! We are not responsible!!!
Серьезное предупреждение! Данная прошивка осуществляет проверку уникального ID устройства, если вы запишите эту прошивку на нелегальное устройство, вы будете нести ответственность за все причиненные убытки! Мы не несем ответственности!!!
심각한 경고! 이 펌웨어는 장치 고유 ID 확인을 수행하며,이 펌웨어를 불법 장치에 구울 경우 발생하는 모든 손해에 대한 책임은 귀하에게 있습니다! 우리는 책임지지 않습니다!!!
重大な警告 このファームウェアはデバイスのユニークID検証を行います。もしこのファームウェアを違法なデバイスに焼いた場合、生じた損害はすべてあなたの責任となります！ 私たちは責任を負いません!
