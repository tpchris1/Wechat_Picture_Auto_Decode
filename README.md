# 微信電腦版圖片解碼器 
Wechat_Picture_Auto_Decode

## Overview
微信電腦版個人目錄下面的各種圖片檔，通過dat加密，轉成jpg檔，可以自動找出decode_hex
## Environment
Jupyter 3 (python 3.7.3)
## Usage
1. 直接download這個script
2. 延伸說明：
    1. 通過[這個](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor)vscode插件可以直接看到dat的16進制
    2. 最前面兩個byte XOR ffd8（一般JPG的最前面兩個byte就是ffd8），得到decode_hex
    3. dat中每一個byte都去除decode_hex，並且output
## Reference
https://blog.csdn.net/u010553139/article/details/103522222