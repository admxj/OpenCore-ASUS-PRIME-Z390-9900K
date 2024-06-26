# OpenCore_ASUS_PRIME_Z390_9900K

## 硬件简介
OpenCore: ASUS PRIME Z390-A + 9900k + RX5700XT

[OpenCore-Desktop-Guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html)

## 系统信息
![system-info.png](./images/system-info.png)
![geekbench-cpu.png](./images/geekbench-cpu.png)
![geekbench-gpu.png](./images/geekbench-gpu.png)
![fans.png](./images/fans.png)
![network.png](./images/network.png)

## **配置**

|  配件  | 型号  | 
|  ---- | ---- | 
|  CPU  | 9900K | 
|  内存  | DDR4 2400 x 4 | 
|  主板  | ASUS）PRIME Z390-A  | 
|  显卡  | (Sapphire)RX 5700 XT 8G D6 |
|  SSD  | Samsung PRO 970 |
|  BT/Wi-Fi  | Broadcom BCM43xx | 


## **EFI**

* boot args `agdpmod=pikera alcid=11`
* 新增ACPI
    - *SSDT-USBX.aml* 
    - *SSDT-PMC.aml*
    - *SSDT-PLUG.aml*
    - *SSDT-EC.aml*
    - *SSDT-AWAC.aml*
* 新增 the HfsPlus.efi driver
* 新增Kexts
    - *WhateverGreen.kext*
    - *VirtualSMC.kext*
    - *SMCSuperIO.kext*
    - *USBPorts.kext*
    - *SMCProcessor.kext*
    - *Lilu.kext*
    - *IntelSnowMausi.kext*
    - *IntelMausi.kext*
    - *AppleALC.kext*
* 关闭`XhciportLimit` 15个USB限制, 自定义USB端口


## **更新日志**

- 2024年06月10日
  - 升级`OpenCore`到1.0.0
  - 新增`Intel 82599`万兆网卡驱动
  - 升级一堆`Kexts`驱动
  - 升级一堆`Driver`驱动

- 2022年10月26日
  - 升级`OpenCore`到8.5
  - 新增`Intel 82599`万兆网卡驱动
  - 升级一堆`Kexts`驱动
  - 升级一堆`Driver`驱动

- 2022年06月03日
  - 升级`OpenCore`到8.0
  - 升级`Kexts`驱动 `AppleALC`到1.7.1
  - 升级`Kexts`驱动 `Lilu`到1.6.0

- 2022年03月31日
  - 升级`OpenCore`到7.9
  - 升级`Kexts`驱动 `AppleALC`到1.7.0
  - 升级`Kexts`驱动 `SMCProcessor`到1.2.9
  - 升级`Kexts`驱动 `SMCSuperIO`到1.2.9
  - 升级`Kexts`驱动 `VirtualSMC`到1.2.9
  - 升级`Kexts`驱动 `WhateverGreen`到1.5.8

- 2021年10月26日
  - 升级`OpenCore`到7.4
  
- 2021年10月25日
    - 升级`Kexts`驱动 `AppleALC`到1.6.5
    - 升级`Kexts`驱动 `Lilu`到1.5.6
    - 升级`Kexts`驱动 `VirtualSMC`到1.2.7
    - 升级`Kexts`驱动 `WhateverGreen`到1.5.4

- 2021年08月17日
    - 升级`OpenCore`到7.2
    - 升级`Kexts`驱动 `IntelSnowMausi`到1.0.7
    - 升级`Kexts`驱动 `AppleALC`到1.6.3
    - 升级`Kexts`驱动 `Lilu`到1.5.5
    - 升级`Kexts`驱动 `VirtualSMC`到1.2.6
    - 升级`Kexts`驱动 `WhateverGreen`到1.5.2
  

- 2021年07月23日
    - 升级`OpenCore`到7.1
    - 升级`Kexts`驱动 `AppleALC`到1.6.2
    - 升级`Kexts`驱动`IntelMausi`到1.0.7
    - 升级`Kexts`驱动`Lilu`到1.5.4
    - 升级`Kexts`驱动`VirtualSMC`到1.2.5
    - 升级`Kexts`驱动`WhateverGreen`到1.5.1

- 2021年05月20日
    - 升级Kexts
    - 升级`OpenCore`到6.9
    - 测试通过bigSur 11.3.1
