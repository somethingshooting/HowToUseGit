# 概要
gitの主に使用するコマンドをまとめたものを掲載したリポジトリ。

# 主に使用するコマンド
### 初めてgitを使用するときの手順
1. `$ git init`  
2. `$ git pull https://... ...` or `$ git clone https://... ...`  
3. `$ git remote add origin https://... ...`
### ブランチの作成や移動
- ブランチを移動するとき  
`$ git checkout [移動先のブランチ名]`
- 新たにブランチを作成するとき  
`$ git checkout -b [作成するブランチ名]`
### 変更したファイルをステージングする
`$ git add [変更したファイル名]`  
- 変更したファイルをすべてステージングする  
`$ git add .`
### ステージングしたファイルをコミットする
- 一行だけメッセージを書く  
`$ git commit -m "[コミットメッセージ]"`  
- 複数行メッセージを書く
`$ git commit`  
`i`を押して挿入モードで記述  
半角モードで`Esc`を押して`:wq`を入力し`Enter`を押せばメッセージを確定できる
### プッシュする
- ブランチで初めてする  
`$ git push -u origin [プッシュするブランチ名]`
- 二回目以降のプッシュをする  
`$ git push`
### GitHub上の情報を取得する
- 情報だけ取得する  
`$ git fetch` or `$ git fetch origin`
- 情報を取得してマージする
`$ git pull` or `$ git pull origin [マージしたいGitHub上のブランチ名]`
### コミットしたくないけどセーブしてブランチを切り替えたい
- セーブするとき  
`$ git stash`  
`$ git checkout [移動先のブランチ名]`  
- セーブデータをロードする  
`$ git stash apply`
### 変更のログを見たい
`$ git log`  
### プルリクエストをしたい
GitHubサイト上のGUIでする  
