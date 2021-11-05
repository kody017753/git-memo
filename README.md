# memo

・gitユーザーの設定
$git config --global user.name "<自分の名前>"
$git config --global user.email "<自分のメアド>"


・ユーザー設定の確認
$git config --global --list


・リモートリポからcloneしてローカルリポを作成する
$git clone <github上のurl>


・ローカルリポに紐づいているリモートリポのURLを確認する
$git remote -v


・ブランチ一覧を表示する（現在のブランチを確認）
$git branch


・新しいブランチを切る（作成する）
$git branch <好きな名前>


・作業するブランチを切り替える
$git checkout <一覧にある名前>
  ※git checkout -b <好きな名前>にすると作成と切り替えが同時にできる
  
  
・作業状態を確認する
$git status
  
  
・作業内容をstaging area に追加する
$git add <内容を変更したファイルの名前>


・staging area の内容をコミットする(セーブするイメージ)
$git commit -m "<変更した内容>"


・コミット履歴を表示する
$git log


・リモートリポの更新をローカルリポに反映する
$git pull <remote_ref(大半「origin」になる)> <branchname(「main」でいい)>
  ※cloneしたあとに誰かがリモートリポを更新しているかもしれないから

・ローカルリポの更新をリモートリポーに反映する
$git push <remote_ref(大半「origin」になる)> <branchname(変更したブランチの名前)>


・特定のブランチを削除する
$git branch -d<削除したい名前>
※mainにマージしてないブランチは削除できない。強制削除する場合は-dでなく-Dを使う
