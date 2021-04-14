# 網頁設計社 課前預習 DAY2
###### tags: `網頁設計社`
### 講師：
- 社長 #貢丸

## Linux Command
:::warning
:loudspeaker: 以下都是會教的東西，那大家也可以先上網查，先預習，這樣對於之後教學時，可以更快的了解講師在講什麼。
※ 以下內容屬於比較簡略，會在課程上進行詳細解說並且補充更多指令 
:::
[TOC]

## Linux 素什麼?
Linux 是一種 Open-source 的類UNIX作業系統核心。
目前最主要的 Linux distributions 含Ubuntu、Debian、Fedora、CentOS等

## Linux Command
在Linux系統中 如果不想用 ui介面進行操作時 我們就可以透過打開terminal 進行指令操作
```
$ 指令 [OPTIONS] [dIR]
```
### cd 移動進入資料夾
進入到david資料夾
```
$ cd ./david
```
移動到根目錄 
```
$ cd /
```
移動到該使用者家目錄
```
$ cd ~
```
返回上一層
```
$ cd ..
```


### mkdir 創建新資料夾
創建
```
mkdir david
```
### ls 查看檔案及子目錄
列出當前目錄的資料
```
$ ls
```
顯示 . 為開頭的資料夾或檔案
```
$ ls –a   
```
詳細內容列出來
```
$ ls –l    
```
### mv 移動檔案或是重新命名檔案
改名 由婚紗照.jpg 改名成西裝照.jpg
```
$ mv 婚紗照.jpg   西裝照.jpg
```
從程式hello.py檔案 移動到程式2裡面
```
$ mv 程式/hello.py   程式2/  
```
如果檔案存在 他會直接強制覆蓋
```
$ mv  程式/  程式2/  -f
```
不會覆蓋任何檔案
```
$ mv  程式/  程式2/  -n
```
### rm 刪除檔案
刪除檔案
```
$ rm hello.cpp
```
刪除目錄
```
$ rm –r 程式2/
```
強制刪除文件和檔案 
```
$ rm –rf 程式2/
```
### wget 下載文件
下載指定網址檔案 –O指定該檔案名稱 
```
$ wget "https://david.jpg" -O david.jpg
```
### cat 將文件印出在終端機上
打印出david.txt裡面的文字
```
$ cat  david.txt
```
### chmod 控制文件或資料夾權限
加入可寫可讀可執行的權限
```
$ chmod  +rwx   hello.cpp
-rwxr-xr-x 1 david david 4 Apr 14 04:34
```
去除可寫可讀可執行的權限
```
$ chmod  -rwx   hello.cpp
---------- 1 david david 4 Apr 14 04:34 123.py
```
### file 查詢檔案
確定檔案類型
```
$ file david.txt
david.txt：UTF – 8 Unicode text
```
### grep 查詢關鍵字
普通的關鍵字來搜尋

```
$ grep 123   hello1.txt  Gunjyo.txt
hello.txt : 123
```
不分大小寫 去搜尋
```
$ grep –i PReTty  hello1.txt  Gunjyo.txt 
Gunjyo.txt： Pretty
```
### nc
查看該port是否有開啟
```
$ 192.168.121.100 22
```
### apt-get 套件管理工具
更新套件資料庫列表
```
$ sudo apt-get update
```
升級套件並下載安裝套件
```
$ sudo apt-get upgrade
```
下載tor的工具
```
$ sudo apt-get install tor
```
### sudo 使用最高權限執行指令
使用最高權限下載 tor的工具
```
$ sudo apt install tor
```
### echo 打印
打印出文字
```
$ echo 貢丸很帥
貢丸很帥
```
