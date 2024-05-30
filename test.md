# GITHUB practice
- *bacic command*

1. 配置
在首次使用 Git 時，你需要配置你的用戶名和電子郵件地址：
- git config --global user.name "Your Name"
- git config --global user.email "your.email@example.com"

## 創建和初始化倉庫
初始化一個新的 Git 倉庫：
- git init
- git clone   (https://github.com/user/repository.git)

基本操作
## 檢查當前倉庫的狀態：
- git status

## 將文件添加到暫存區：
- git add filename
## 或者添加所有更改的文件
- git add 
## 提交更改：
- git commit -m "描述提交的更改"
## 查看提交歷史：
- git log
- git log --oneline
- git config --list

## 比對版本差異
- git diff "版本ID" "檔案名"

# 分支操作
## 查看當前所有分支：
- git branch
## 創建新分支：
- git branch new-branch

##　切換到新分支：
- git checkout new-branch

## 創建並切換到新分支：
- git checkout -b new-branch

## 合併分支：
- git checkout main
- git merge new-branch

## 刪除分支：
- git branch -d new-branch

# 遠端操作
## 添加遠端倉庫：
- git remote add origin (https://github.com/user/repository.git)

## 查看遠端倉庫：
- git remote -v

## 從遠端倉庫拉取更改：
- git pull origin main

## 推送更改到遠端倉庫：
- git push origin main

# 標籤
## 創建標籤：
- git tag v1.0

## 推送標籤到遠端倉庫：
- git push origin v1.0

## 查看所有標籤：
- git tag

# 撤銷操作

## 取消暫存區的更改：
- git reset HEAD filename

## 取消工作區的更改：
- git checkout "版本ID" -- 檔案名
  *回溯完後必須再 git commit -m "修改說明"* 
  這種作法會留下全部的修改歷程
## 回退到某個提交：
- git revert commit_hash

## 強制回退到某個提交：
- git reset --hard "版本ID"
  這個做法會回溯到某個還原點並刪除該點之後的紀錄

# GIT 文件狀態
- Untracked   未追蹤
- Tracked     追蹤
- Staged      已暫存
- Committed   已提交

# 忽略不需要追蹤版本的文件
- 建立一個檔名為".gitignore"的檔案，將要忽略的檔案名稱寫在裡面 EX:*.json

![開啟圖片](https://static.jyshare.com/images/runoob-logo.png "圖片")

![圖片](https://octodex.github.com/images/bannekat.png "圖片")
