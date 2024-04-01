# react-on-GitHub-pages--test
react-on-GitHub-pages 

https://www.youtube.com/watch?v=AkHWdHYa9Vs
https://www.youtube.com/watch?v=gtODigNB6Is


## Getting Started Github
1. create repository: 
2. Add collaborators to this repository:Invite collaborators
3. Check your inbox for collaboration notifications and confirm. 


## To run the project locally:
1. Clone this repository: `git clone https://github.com/Amity0317/react-on-GitHub-pages-test.git`or 使用vscode的複製
2. Install dependencies: `npm install`
3. 建立react專案(專案名稱須都小寫react-on-githubpages): `npx create-react-app react-on-githubpages`
3. 因gthub靜態檔根目錄需求，將專案react-on-githubpages內層資料移至最外層(node_modules除外)，react-on-githubpages資料夾刪除，在外層重新 `npm install`
4. 安裝 gh-pages package ： `npm install gh-pages --save-dev`
5. package.json 
```javascript
   "homepage": "https://amity0317.github.io/react-on-GitHub-pages-test",
```

6. package.json
```javascript
  "scripts": {
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build",
  },
```
7. 確認專案正常運作: `npm start`
8. (如果使用vscode的複製，需重新使用`git init`)，創建新分支:git checkout -b gh-pages
9. git push -u origin gh-pages:  -u 用於設置遠端分支和本地分支之間的關聯。當你使用 -u 選項推送分支時，Git 將會記住該遠端分支，之後你可以使用 git push 命令而不需要再指定遠端分支名。
10. 前往 Github 的設定把預設分支設成 gh-pages 並把儲存庫設為公開，Settings/pages/Branch:將公開的頁面branch指向gh-pages>save，重新整理頁面將得到展示網址(Your site is live at):
[https://amity0317.github.io/react-on-GitHub-pages--test/react-on-github-pages/](https://amity0317.github.io/react-on-GitHub-pages--test/react-on-github-pages/)



