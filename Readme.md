# github startup
基本的に、ローカルリポジトリに変更を追加していき、最後にリモートに追加するイメージ


## 初期手順
1. ワーキングディレクトリを作成し、git init
   - 初期化

2. 作成したファイルをローカルリポジトリにためる
   - git add file
   - git commit -m "first commit"

3. どこのrepositoryにコミットするかを選択(最初だけ)
   - git remote add origin https:~

4. git push origin master

## すでにあるリポジトリからpull
1. git init
2. git remote add origin https:~
3. git pull origin master

### 注意
* 先にReadmeを作成している場合は、先にpullする必要がある。
* git pull = git fetch + git merge origin/master


## branch
- git branch 
   - 現在のブランチ一覧を表示
- git branch name
   - nameブランチを作成
- git checkout name
   - nameブランチに切り替え

## pull reqへの道のり
```
作業途中でremoteのmasterが変わってしまった場合
```
1. もし、作業途中のものでcommit出来るものがあればcommitしておく
2. masterブランチへ移動
   - git checkout master
3. git pullでmasterを最新に
   - git pull origin master
4. 開発用ブランチへ移動
   - git checkout 開発用ブランチ
5. mergeコマンドでmaserの内容を取り込む
   - git merge origin/master
