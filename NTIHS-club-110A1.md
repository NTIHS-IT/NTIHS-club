# 網頁設計社 課前預習 DAY1 (110上)
###### tags: `網頁設計社`
[TOC]
## 講師:
- Young#0001<!-- 社長我愛你QwQ -->
# 終端機 Terminal
:::warning
:loudspeaker: 以下都是會教的東西，那大家也可以先上網查，先預習，這樣對於之後教學時，可以更快的了解講師在講什麼。
::: 
終端機是早期電腦常見的輸入輸出介面  
簡單來說就是以前電腦的一切操作都是在終端機內輸入指令來達成  
現在的終端機大部分功能雖然都已經被圖形化介面取代了  
但是實際操作終端機後可以對電腦做更進一步的控制  
這節課會介紹 Windows 終端機的使用方法  

以下講解內容皆為 Windows Terminal  
不同系統的終端機語法會有些微的差別  

![](https://i.imgur.com/MGNOd40.jpg)

## 檔案儲存結構
接下來要介紹切換目錄的 cd 指令  
所以先講檔案的儲存結構  
Windows 儲存檔案的方式是以樹狀結構儲存檔案  
所以會有一層一層的資料夾  

如下圖:  

![](https://i.imgur.com/qb374Vj.png)

## 使用管理員身分開啟 Terminal
### 優缺點
以管理員身分啟動 Terminal 可以使用系統中更完整的功能  
但是第一次碰終端機的話 例如誤刪重要資料  
### 使用方法
使用 Windows 中的啟動快速鍵 Win + R  
輸入 cmd  
按下 ctrl + shift + enter  
就可以快速以管理員身分啟動 cmd  
如果不使用管理員身分就輸入 cmd 以後直接按下 enter  
## 系統內建指令
### help
help 很好懂  
就是把所有的指令和功能列出來  

![](https://i.imgur.com/0q8Et47.png)

只截一部份的指令出來  
因為量太多了  
### cd
更改當前所在的資料夾位置  
- 進入指定資料夾
```
cd (資料夾名稱)
```  
- 返回上一層資料夾
```
cd ..
```  
#### 一次移動多層
假如這是我們目前所在的目錄  
```
C:\Users\Young\b
```  
如果要移動到  
```
C:\Users\Young\a
```  
可以直接使用  
```
cd ../b
```  

![](https://i.imgur.com/W4dtwXy.png)

### dir
查看當前資料夾下所有檔案和資料夾  
會列出磁碟名稱 磁碟區序號  
檔案數量 檔案大小  
#### 使用方法

```
dir
```

![](https://i.imgur.com/RlYCSpb.png)

### mkdir
建立資料夾  
#### 使用方法
```
mkdir (資料夾名稱)
```  

![](https://i.imgur.com/7G7ukdI.png)

新增資料夾後使用剛剛的```cd```進入資料夾確認已新增  
### copy
複製檔案  
#### 使用方法
```
copy (要複製的檔案名稱) (複製完成的檔案名稱)
```  

![](https://i.imgur.com/wIwFwp9.png)
### move
移動檔案  

這邊的 move 只講解移動檔案  
不考慮重複檔案名稱和移動資料夾的問題  
#### 使用方法
```
move 檔案名稱(可輸入絕對位置 or 相對位置) 檔案(可輸入絕對位置 or 相對位置)
```  

直接看可能有點難理解  
所以以下附圖片說明  

首先我們的```C:\Users\Young\a```內有一個檔案  
名稱叫做```a.txt```  
先使用 ```dir``` 檢查資料夾的檔案  
```
dir
```
![](https://i.imgur.com/aLAeg0t.png)

要將```a.txt```移動到```C:\Users\Young\b```  
(回到上一層->進入資料夾`b`)  
```
move a.txt ../b
```
![](https://i.imgur.com/nqBQfMM.png)

切換目前所在目錄  
```
cd ../b
```
![](https://i.imgur.com/QiSEill.png)

檢查資料夾`b`裡面的檔案  
```
dir
```
![](https://i.imgur.com/DODRdC1.png)

可以發現```a.txt```已經成功從  
資料夾`a`移動到資料夾`b`  
#### 使用方法
### del
刪除檔案  
#### 使用方法
```
del (檔案名稱)
```  

![](https://i.imgur.com/PZ2pA2H.png)

### cls
清空畫面  
#### 使用方法
```
cls
```
使用後的螢幕上只剩下C:\Users\Young\a>  

![](https://i.imgur.com/OcGJxRg.png)

### ping
測試網路通道是否開啟  
常用於測試網站和伺服器  
#### 使用方法
```
ping (DNS位址 or ip)
```  

![](https://i.imgur.com/xsGALkq.png)

ping 預設是 ping 四次  

正在 ping 的時候會顯示的有  
1. 傳回封包的 ip  
2. 每次傳送的封包大小  
3. 每次傳回來的時間  
4. TTL(Time to Live)  
(還可以被轉發多少次)  

ping 結束後會印出的有  
1. 傳回封包的來源 ip  
2. 已傳送 接收 遺失的封包數量  
3. 傳回封包的最短時間 最長時間 平均時間 (ms)  
## 延伸套件
### Python pip
Python 中的 pip 提供了方便的套件安裝方法  
每個套件都有不同的功能  
可以直接從 pip 安裝來用  
#### 安裝pip
pip 要在安裝 python 的時候同時裝  
以下為安裝 pip 的步驟  
1. 到 Python 官方網站下載 Python 安裝程式
2. 啟動 Python 的安裝程式
3. 勾選 Add Python (版本名稱) to Path  
4. 選擇 Install Now  

安裝完成後可以開啟 cmd  
```
pip
```

![](https://i.imgur.com/PSXoLHG.png)
```
pip --version
```
![](https://i.imgur.com/ZFEz6GE.png)
```
python --version
```
![](https://i.imgur.com/rhBMMgk.png)

#### pip install
從名稱來看很明顯就是安裝套件  
那就直接實作吧  
#### 使用方法
```
pip install (套件名稱)
```
![](https://i.imgur.com/1bNkZ6S.png)

#### pip list
列出所有的套件名稱和版本  
#### 使用方法
```
pip list
```
![](https://i.imgur.com/mftAyy3.png)

#### pip uninstall
剛剛看完了 pip install  
現在看 uninstall  
很明顯是解除安裝套件  
#### 使用方法
```
pip uninstall (套件名稱)
```
![](https://i.imgur.com/NMCzsJ0.png)

#### youtube-dl
youtube-dl 是一個快速下載 Youtube 影片的 Python 專案  
我們可以直接使用 pip 將它安裝在自己的電腦上  
如同前面示範 pip install 的用法  
那安裝 youtube-dl 之後我們可以直接輸入 youtube-dl  
檢查套件的安裝情況  

![](https://i.imgur.com/a7e4aKO.png)

看到它介紹套件的使用方法代表套件已經可以使用了  
#### 使用方法
```
youtube-dl (影片連結)
```
![](https://i.imgur.com/lqi6MqD.png)

### git
git 是一種版本控制系統  
用來管理專案的版本  
下一節社課會更深入介紹  
敬請期待  