
sitoryに行くとすべての変更が見れる
    - 変えたいところだけローカルで変える事ができる

- set config values
```
  962* git config --global user.name hogehoge
  963* git config --global user.email fugafuga
```
## local
- git init
> Initialized empty Git repository in /home/imaimai/Documents/gitutorial/.git/
    - .git directoryがデキる
    - 消すときはrm -rf .git
- git status
    - 今どういう状態にいるかを確認する
    - untracked files
- touch .gitignore
    - addなどtrackingしたくないファイルに関してはここに書く
- git add <files>
    - working directory(localの作業場)--add-->Staging Area
    - Staging Area --commit-->.git directory
    - git add -A : すべてのファイル(.gitignoreは除く)をadd
    - changes to be commited:に追加される
- git commit -m "hogehoge"
    - ステージされているものを.gitにあげる
    - -mをすると、一行コメントを残せる("hogehoge")
    - working directory clean となる
- git log
    - commitのハッシュ番号、author,date,commentがログとしてみられる


## project with team
- git clone <url> <cloneしたい場所>
    - 場所を省略すると、その場所に鳴る
- git remote -v
    - リポジトリの情報が載る(取ってくるurl, 更新のときに使うurl)
- git branch -a
    - リポジトリのブランチリストが全て載る
- git push origin master
-

