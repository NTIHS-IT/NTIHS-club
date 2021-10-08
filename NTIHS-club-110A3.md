---
tags: 網頁設計社
---

# 網頁設計社 課前預習 DAY3 (110上)

[TOC]
## 講師:
- Young#0001
# 版本控制系統 Git
:::warning
:loudspeaker: 以下都是會教的東西，那大家也可以先上網查，先預習，這樣對於之後教學時，可以更快的了解講師在講什麼。
:::
## Git 基本介紹
git 是一種版本控制系統  
目前很多大型的開源專案都是使用 git 來管理  
但是對於個人的專案管理也很方便  
github 提供了 git 好理解和操作的圖形化介面  
這節課會介紹 git 和 github 的基本使用方法  

git 在終端機內的功能大概有這些  
![](https://cdn.discordapp.com/attachments/711916752551804989/853990905169182750/unknown.png)

## Git 概念

![](https://i.imgur.com/cmohFs0.png)

## Git 使用方法
接下來會一步一步帶大家用終端機來操作 git  
主要流程:
1. 建立 repository
2. commit
3. remote add
4. Push 到 Github

## 新增 Git repository
1. 進入 windows cmd 或 linux terminal  
2. 建立並進到一個空的資料夾內  (mkdir & cd)
3. 輸入 git init  

```shell=
git init
```

這樣你的 Git repository 就已經建立好了  

## Git add

將檔案加入版本控制追蹤名單  
使用方法:  

```shell=
git add [檔案名稱]
```

如果要把當前的目錄底下所有檔案  
都加入版本控制的話可以使用  

```shell=
git add .
```

## Git commit
commit 可以把寫好並且有被添加(git add)  
到版本管理的程式加到 Git 內  

```shell=
git commit -m "這是一個commit"
```

## Push 到 Github
Github 是一個以 git 為基礎架設的網路服務平台  
Github 比起終端機內的 git 更加好理解  
我們可以直接下載 Github 的桌面版 [Github Desktop](https://desktop.github.com)   

在 push 之前我們要先有一個雲端的 Git 服務  
並且設定好 push 的目的地  

## 申請 Github 帳號

直接在瀏覽器搜尋 Github  
然後辦好一個帳號  
這邊就先不教如何辦 Github 帳號  

## 新增雲端庫

在 Github 上點擊  
Profile > Repositories > new repository  

![](https://i.imgur.com/pyZuRGF.png)

取好名稱後就直接新增  
然後會看到以下畫面  

![](https://i.imgur.com/Nn12FX2.png)

這樣就新增好雲端庫了  
然後複製上面的連結  
等一下會用到  

## Git remote add

把本機的 repository 連結到雲端的 Github 庫  

```shell=
git remote add [遠端庫簡稱 可以自己取] [Github上的連結]
```

## Git push

最後我們終於要 Push 到 Github 上了  
首先先把剛剛的遠端庫簡稱設定到 Github 的 main 分支上  

```shell=
git push -u [遠端庫簡稱] main
```

main 是預設的分支  
有關 Github 分支的用法可以上網查  
`Github branch`  
這邊就不贅述  

## 新增一個檔案後再 Push 到 Github 一次

前面已經把我們第一個 commit push 到 Github 上的儲存庫了  
那之後我們變動檔案完要再 Push 就不會那麼麻煩了  
只剩下三個步驟  

```shell=
git add .
git commit -m "這是一個commit"
git push
```

## Git ignore

如果我們有些檔案不想推到 Github 上的話  
例如編譯好的 exe 檔案  
我們可以新增一個檔案取名叫`.gitignore`  

![](https://i.imgur.com/nJDLmm9.png)

然後開啟它以後寫上`*.exe`  

## 加入我們的 Github organization

我們社團有自己的 Github 組織  
歡迎各位加入  
只要進到 Discord 伺服器留下自己的 Github 使用者名稱  
就會邀請你加入 Github 組織  

![](https://cdn.discordapp.com/attachments/878632791728869401/884689392323678239/JH1ZhmiAgFEFOxqzQPI1SourjeAiIJdrXkAuVrFxfUGEFGwqzUPIFeruLjeACIKdrXmAeRqFRfXxYfz8dJXtW4QAAAABJRU5ErkJ.png)