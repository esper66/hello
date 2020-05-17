# github startup
基本的に、ローカルリポジトリに変更を追加していき、最後にリモートに追加するイメージ


1. ワーキングディレクトリを作成し、git init
   - 初期化

2. 作成したファイルをローカルリポジトリにためる
   - git add newfile
   - git commit -m "first commit"

3. どこのrepositoryにコミットするかを選択
   - git remote add origin https:~

4. git push origin master



### 注意
* 先にReadmeを作成している場合は、先にpullする必要がある。
* git pull = git fetch + git merge origin/master