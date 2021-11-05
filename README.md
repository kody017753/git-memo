# memo

gitの基本

gitユーザーの設定
$git config --global user.name "<自分の名前>"
$git config --global user.email "<自分のメアド>"



ユーザー設定の確認
$git config --global --list



リモートリポからcloneしてローカルリポを作成する
$git clone <github上のurl>

ローカルリポに紐づいているリモートリポのURLを確認する
$git remote -v

ブランチ一覧を表示する（現在のブランチを確認）
$git branch

新しいブランチを切る（作成する）
$git branch <好きな名前>

作業するブランチを切り替える
$git checkout <一覧にある名前>
  ※git checkout -b <好きな名前>にすると作成と切り替えが同時にできる
  
  作業状態を確認する
  $git status
  
  作業内容をstaging area に追加する
  $git add 
