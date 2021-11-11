

## gitユーザーの設定
```bash
git config --global user.name "<自分の名前>"
git config --global user.email "<自分のメアド>"
```


## ユーザー設定の確認
```bash
git config --global --list
```

## リモートリポからcloneしてローカルリポを作成
```bash
git clone <github上のurl>
```

## ローカルリポに紐づいているリモートリポのURLを確認
```bash
git remote -v
```

## ブランチ一覧を表示（現在のブランチを確認）
```bash
git branch
```

## 新しいブランチを切る（作成する）
```bash
git branch <好きな名前>
```

## 作業するブランチを切り替える
```bash
git checkout <一覧にある名前>
 ※git checkout -b <好きな名前>にすると作成と切り替えが同時にできる
 ```
  
  
## 作業状態を確認
```bash
git status
```  
  
## 作業内容をstaging area に追加
```bash
git add <内容を変更したファイルの名前>
```

## staging area の内容をコミットする(セーブするイメージ)
```bash
git commit -m "<変更した内容>"
```

## コミット履歴を表示
```bash
git log
```

## リモートリポの更新をローカルリポに反映する
```bash
git pull <remote_ref(大半「origin」になる)> <branchname(「main」でいい)>
 ※cloneしたあとに誰かがリモートリポを更新しているかもしれないため
```

## ローカルリポの更新をリモートリポに反映する
```bash
git push <remote_ref(大半「origin」になる)> <branchname(変更したブランチの名前)>
```

## 特定のブランチを削除する
```bash
git branch -d<削除したい名前>
※mainにマージしてないブランチは削除できない。強制削除する場合は-dでなく-Dを使う
```
