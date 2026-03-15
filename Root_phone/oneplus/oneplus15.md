手機:oneplus 15 (一加15) 版本 CN->EU(轉歐盟版)  
價格:25K NT 含稅 約27K  
規格:16G/1TB  

買大陸手機的原因:  
這個規格你在台灣買要4萬    
**注意 網路頻段會有所減少**  
我目前無法使用B28(700)頻段 已經改了EFS文件也一樣

先去oneplus官網下載 深度申請測試    
每天早上凌晨 2:00 通過申請測試    

申請測試後 刷入橘狐(https://xdaforums.com/t/oneplus-15-custom-roms.4767379/)  
  
進去fastboot 刷入該recovery  
把CN 轉區ROM包 載入手機  
在該recovrey刷入ROM包(我這邊2分鐘內)  
**!! 請注意 請先備分所有區塊 !!**  

**!! 尤其是這些區塊 特別重要 這是手機的身分證 沒有你就無法上網 !!**  
!! persist modem efs1/2 efsc efsg !!  

然後 清除data 開機 完畢  

刷氧成功~  

-> **!這時候有兩條分支!**  

## OTA升級後 上BL鎖  
->  
下載官方安裝OTA包 我懶得找 你要自己找  
強制本地安裝 A/B欄位都需相同  
然後進去fastboot模式 上鎖定  
!!注意 如果你不是原本ROM 會被紅色鎖定 這是無法被解鎖的!!  
!!只能去售後 除非你人在大陸 不然不建議 或者你知道你在做甚麼!!  


## 保留ROOT  
保留root 可以參考 **KernelSU**  
  
我使用分支  
KernelSU-Next  
更好的隱藏跟支援  

使用自訂義內核  
(https://github.com/WildKernels/OnePlus_KernelSU_SUSFS/releases/tag/v2.0.0-r6)  
(在recovery刷入即可)  
 
然後安裝  
KernelSU-Next  

好 完畢  

KSU是甚麼?  
root管理器 內核等級隱藏 只會主動給予Root權限 不會被動給予(magisk)  
  
安裝APP  
{  
KernelSU_Next_v3.0.0_32857-release  
KsuWebUI-1.0-34-release  
HMA-V3.6.1.r462.4524dde-release  
}
  
再來刷入隱藏與繞過模塊即可  
{  
ksu_module_susfs_1.5.2+  
Zygisk-Next-1.3.2-688-2c60cdd-release  
LSPosed-v1.10.2-7182-zygisk-release  
PlayIntegrityFix_v4.4-inject-s  
Tricky-Store-v1.4.1-245-72b2e84-release  
TrickyAddonModule-v4.3  
}請按照順序安裝  


好 目前root就完畢了  


等我有時間再更新GPU降壓~   
