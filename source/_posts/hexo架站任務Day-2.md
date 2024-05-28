---
title: hexo架站任務Day-2
date: 2024-05-24 09:45:54
tags:
    -學習歷程第二天
---

# 將架設好的Hexo部屬到GitHub

<!--more-->

## 第一步：將GitHub綁到VSCode
待更新

## 第二步：在GitHub上建立一個新的 Repositories
待更新

## 第三步：一鍵部署
1. 安裝[hexo-deployer-git](https://github.com/hexojs/hexo-deployer-git)
```
npm install hexo-deployer-git --save
```
2.清空_config.yml裡 deploy現有資料，並取代成以下組態：
```
deploy:
    type: git
    repo: https://github.com/<username>/<project>
    # example, https://github.com/hexojs/hexojs.github.io
    branch: gh-pages
```
其中 username = github使用者名稱；project = 專案名稱
3. 執行以下指令：
```
hexo clean && hexo deploy
```
<注意>若此時報錯資訊為不支援 "&&"符號，則改成 ";"就可以解決
4. 執行完後，檢查是否執行 https://username.github.io/project/