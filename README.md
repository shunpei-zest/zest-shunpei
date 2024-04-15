# ローカル作業
---
## リポジトリのセットアップ
- `git@github.com:shunpei-zest/zest-shunpei.git`
## ブランチの作成
1. `git branch switch main` -> mainブランチへ移動
2. `git pull origin main` -> mainブランチをローカルへ同期
3. `git switch -c ZEST-xxx_do_something` -> 新規ブランチ作成
## リポジトリの更新作業
1. ファイルの編集
2. `git add .` -> 指定したファイルをインデックスに登録してコミット対象にする
3. `git commit -m "ZEST-xxx yyyのためにzzzした"` -> 追加・変更したファイルをGitに登録
4. `git push -u origin ZEST-xxx_do_something` -> ローカルで変更したブランチをリモートに送信(`-u`コマンドを入れることで、以降のローカルからリモートへのpushの際には、リポジトリ名を省略することが可能)
## さらにファイル編集したい場合は以下を繰り返す
1. （mainを取り込みたい場合）`git pull --rebase origin main`
2. ファイルの編集
3. `git add .`
4. `git commit -m "ZEST-xxx yyyのためにzzzした"`
5. `git push`