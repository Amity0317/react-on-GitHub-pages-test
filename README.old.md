# react-on-GitHub-pages--test
react-on-GitHub-pages 

https://www.youtube.com/watch?v=AkHWdHYa9Vs
https://www.youtube.com/watch?v=gtODigNB6Is
https://www.youtube.com/watch?v=zuEvFo-PM5o


## Getting Started Github
1. create repository: 
2. Add collaborators to this repository:Invite collaborators
3. Check your inbox for collaboration notifications and confirm. 


## To run the project locally:
1. Clone this repository: `git clone https://github.com/Amity0317/react-on-GitHub-pages-test.git`or 使用vscode的複製
2. Install dependencies: `npm install`
3. 建立react專案(專案名稱須都小寫react-on-githubpages): `npx create-react-app react-on-githubpages`
4. 因gthub靜態檔根目錄需求，將專案react-on-githubpages內層資料移至最外層(node_modules除外)，react-on-githubpages資料夾刪除，在外層重新 `npm install`
5. 安裝 gh-pages package ： `npm install gh-pages --save-dev`
6. package.json 
```javascript
   "homepage": "https://amity0317.github.io/react-on-GitHub-pages-test",
```

7. package.json
```javascript
  "scripts": {
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build",
  },
```
8. 確認專案正常運作: `npm start`
9. 如果使用vscode的複製，需重新使用`git init`，創建新分支:`git checkout -b gh-pages`
10. 確認本地儲存庫中是否已設置了遠端儲存庫，可以使用以下命令檢查：`git remote -v`，如果沒有顯示任何遠端儲存庫，您需要添加一個遠端儲存庫，例如：`git remote add origin git@github.com:Amity0317/react-on-GitHub-pages-test.git`(錯了:`git remote remove origin`，改為:`git remote add origin https://github.com/Amity0317/react-on-GitHub-pages-test.git` )
11. `git push -u origin gh-pages`:  -u 用於設置遠端分支和本地分支之間的關聯。當你使用 -u 選項推送分支時，Git 將會記住該遠端分支，之後你可以使用 git push 命令而不需要再指定遠端分支名。
12. 前往 Github 的設定把預設分支設成 gh-pages 並把儲存庫設為公開，Settings/pages/Branch:將公開的頁面branch指向gh-pages>save，重新整理頁面將得到展示網址(Your site is live at):
[https://amity0317.github.io/react-on-GitHub-pages-test/](https://amity0317.github.io/react-on-GitHub-pages-test/)(尚無部署)
13. `npm run deploy`要等一下，而在github-專案/右側deployments/[https://amity0317.github.io/react-on-GitHub-pages-test/](https://amity0317.github.io/react-on-GitHub-pages-test/)view deployment

PS.不小心push 錯的commit 請執行`git revert cf2d3c1acd21b802efeebef6`+`git push -f origin gh-pages`
然後重新執行`npm install`+`npm start`+`npm install gh-pages --save-dev`+`npm run deploy`

