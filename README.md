# conoha-gh-actions-hugo
http://hayapi.conohawing.com/


## 作成するファイル
ファイル名：`（会社名）-（社員番号）-（名前）.md`

```
---
title: "（会社名）-（社員番号）-（名前）"
date: 2020-05-07T02:00:04+09:00
draft: false
---

## 自己紹介
- 会社名
- 社員番号
- 名前

```

### 開発の流れ

1. [pepabo/conoha-gh-actions-hugo](https://github.com/pepabo/conoha-gh-actions-hugo) を個人のGitHubにフォークする
![fork](https://media.git.pepabo.com/user/948/files/49ac5180-8945-11ea-8b22-049aec36e542)

2. リポジトリをローカルマシンにclone
```
git clone git@github.com:hayasaki-shunsuke/conoha-gh-actions-hugo.git
cd conoha-gh-actions-hugo
```
3. ローカルで修正用ブランチを切る
```
git checkout -b pepabo-hayasaki
```
4. `（会社名）-（社員番号）-（名前）.md`を作成
```
touch content/posts/pepabo-552-hayasaki.md
```
5. 内容を修正する
```text:sample
---
title: "（会社名）（社員番号）（名前）"
date: 2020-05-07T02:00:04+09:00
draft: false
---

## 自己紹介
- 会社名
- 社員番号
- 名前
```
6. 修正をcommitして、ブランチをGitHubにpushする
```
git add content/posts/pepabo-552-hayasaki.md
git commit -m "hayasakiのファイルを追加"
git push --set-upstream origin pepabo-hayasaki
```
7. GitHub上でPull Requestを作成する
![image](https://user-images.githubusercontent.com/48468109/80787280-11b14280-8bc1-11ea-93ef-7c1c5280607a.png)

8. レビューを依頼する

9. レビューがOKならmasterブランチにmergeする
![image](https://user-images.githubusercontent.com/48468109/80786900-f4c83f80-8bbf-11ea-96f9-7c1810e10d92.png)

10.  [本番環境](http://hayapi.conohawing.com/)で確認する
![image](https://user-images.githubusercontent.com/48468109/80785859-af564300-8bbc-11ea-9f3b-56e3f51d7791.png)

