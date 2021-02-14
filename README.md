# Ryzentosh for B550M Pro4
## 仕様
| **構成** | **モデル** |
| ------------- | --------- |
| CPU | AMD Ryzen 5 3600 @ 3.6GHz |
| マザーボード |  ASRock B550M PRO4 |
| RAM | 16GB (2 x 8GB) CORSAIR DDR4-2666MHz |
| オーディオチップセット | Realtek ALC1200 |
| GPU | SAPPHIRE RADEON RX 5500 XT 4GB |
| WiFi | BCM94360NG |
| SSD | ADATA SSD 240GB SU650 |

**macOS version**: 11.2.1 (20D74)  
**OpenCore version**: 0.6.6  

## 動作確認済み
 - Big Sur (11.x)

## 問題点
 - 部分的に機能する仮想化
 - 3.5mmジャックマイクが機能しない
 - スリープが不安定(うまくスリープできない)
## SMBIOS
 - SMBIOSはOpenCore Configuratorなどを使って変更してください(iMacPro 1,1を指定してください)

## SSDT-UIAC.amlとUSBPorts.kext
 `SSDT-UIAC.aml`と`USBPorts.kext`でLEDコントローラーを無効にしています。  
 奇妙なことに無効化しないで`シャットダウン、再起動、スリープ`をすると、画面がブラックアウトしたままBIOSまで立ち上がらなくなります
