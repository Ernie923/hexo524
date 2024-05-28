---
title: hexo架站任務Day-1
date: 2024-05-24 09:45:51
tags:
    -學習歷程第一天
---

參加2024年六角體驗營，才知道原來有這麼方便快速的免費部落格架站框架Hexo
以下為實作小心得
<!--more-->
# han學習Hexo架站初階心得

## 第一步：安裝必要套件
1. 安裝Node.js
首先到[Node.js官網](https://nodejs.org/en/download/prebuilt-installer/current)，選擇LTS版 (比較穩定)

2. 安裝Git
請參考[Git下載連結](https://git-scm.com/downloads)
![](images/git.jpg)

3. 上圖中，以Windows為例，點選電腦中Download for Windows，之後一直無腦下一步即可

4. 可開啟Visual Studio Code，點選 view -> Terminal 啟動終端機

5. 分別輸入
```
node -v
npm -v
git -v
```
若有出現版本號及相關資訊，就代表安裝成功


## 第二步：常用指令
```
hexo init "網站名稱"       --專案初始化及建立
hexo new "部落格名稱"      --新增一篇文章
hexo new page "頁面名稱"   --新增頁面 
hexo generate             --將md檔編譯成HTML格式
hexo server               --啟動伺服器
hexo clean                --清除快取
hexo deploy               --網站部署
```


## 插入圖片
1. 在source資料夾底下，新增「images」資料夾
2. 進入專案的 _config.yml
3. 找到 #Writing區塊
4. 修改 post_asset_folder: true (預設為false)
5. 在新增marked設定，如下圖
![](images/pic_config.jpg)
