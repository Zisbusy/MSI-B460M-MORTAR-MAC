# MSI B460M MORTAR 黑苹果 引导文件

 - MSI B460M MORTAR
 - i5-10500
 - Fenvi FV-T919 BCM94360CD
 - 5500XT

## 注意
从 5.5 以后的版本开始不再支持集显，集显用户可以按以下提示进行修改。
1. 修改集成显卡缓冲帧 AAPL,ig-platform-id 的值为 BwCbPg==
2. 删除注入的5500xt防黑屏参数 agdpmod=pikera


## 安装
本引导高度依据个人喜好修改，默认无oc启动界面。请自行添加三码。     
适用系统：Ventura、Big Sur、Monterey。  

## BIOS设置 

高级-唤醒事件设置     
 - USB设备从S3/S4/S5唤醒：允许     
 - PS/2鼠标从S3/S4/S5唤醒：允许     
 - PS/2键盘从S3/S4/S5唤醒：任意键    

高级-内建显示配置     
 - 集成显卡多显示器：允许（否则核显硬件解码失效，只使用核显的可以忽略）     

OC CPU 特征     
 - OC -> CPU 特征 -> Intel 虚拟化技术：允许     
 - OC -> CPU 特征 -> Intel VT-D 技术：禁止     
 - OC -> CPU 特征 -> CFG锁定：禁止     

安全-安全引导     
 - 安全启动：禁止     

高级     
 - D.T.M 开启     

## 日志
2024-05-02    
 - 升级OC、驱动版本。    

2023-12-11    
 - 关闭 ResizeAppleGpuBars    

2023-06-15    
 - 升级 OpenCore 0.9.3    
 - 升级 Kexts    

2023-06-05    
 - 升级 OpenCore 0.9.2    
 - 升级 Kexts    
 - 取消 5500xt 注入    
 - 优化 原生电源管理 去除 SSDT-PLUG    
 - 优化 B460m专用声卡ID 52    
 
2023-02-12    
 - 升级 OpenCore 0.8.8    
 - 升级 Kexts    
 - 支持 5500xt    
 
2023-01-02    
 - 升级 OpenCore 0.8.7    
 - 升级 Kexts    
 - 支持 5500xt    
 
2022-12-05    
 - 优化显示参数    
 - 优化虚拟化支持    
 - 优化睡眠    
 
2022-11-02    
 - 升级 OpenCore 0.8.5    
 - 升级 WhateverGreen-1.6.1    
 - 升级 VirtualSMC-1.3.0    
 - 升级 Lilu-1.6.2    
 - 升级 AppleALC-1.7.5     
 - 升级 NVMeFix-1.1.0     

2022-05-04    
 - 升级 OpenCore 0.8.0    
 - 升级 WhateverGreen-1.5.8    
 - 升级 VirtualSMC-1.2.9    
 - 升级 Lilu-1.6.0    
 - 升级 AppleALC-1.7.1     
 - 优化 删除大量未启用的配置代码     

2022-04-02    
 - 修复不能检测系统更新bug    

2022-01-24    
 - 取消 HDMI DP 音频输出的屏蔽    
 - 取消 引导扫描限制    
 - 优化 OC 对 Win 的引导支持    

2021-11-18    
 - 升级 OpenCore 0.7.5    
 - 升级 WhateverGreen-1.5.5    
 - 升级 VirtualSMC-1.2.7    
 - 升级 NVMeFix-1.0.9    
 - 升级 Lilu-1.5.7    
 - 升级 AppleALC-1.6.6    
 - 升级 LucyRTL8125Ethernet-1.1.0d12    

## 感谢
https://github.com/acidanthera/OpenCorePkg   
https://github.com/acidanthera/WhateverGreen    
https://github.com/acidanthera/VirtualSMC    
https://github.com/acidanthera/NVMeFix    
https://github.com/acidanthera/Lilu       
https://github.com/acidanthera/AppleALC    
https://github.com/Mieze/LucyRTL8125Ethernet    
https://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1861472
