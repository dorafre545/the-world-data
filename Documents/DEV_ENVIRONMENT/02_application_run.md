# 開発環境動作手順
## Git Clone
ローカルで作業する為、当リポジトリの内容をGitHubからCloneする必要がある。  
作業用ディレクトリにてターミナル等を開き、以下を実行する。  
```git clone git@github.com:dorafre545/the-world-data.git```
エラー等発生しなければ、次の手順へ。

## VSCodeでフォルダを開く
VSCodeを起動し、```Ctrl + K → O```と押下し、フォルダを開くダイアログにてGit Cloneしたディレクトリを開く

## Docker Compose Up
VSCode上にて、```Docker```フォルダ内の```docker-compose.yml```を右クリックし```Compose Up```を押下する。  
エラー等発生しなければ、次の手順へ。

## Dev Container
VSCodeのサイドバーに```Remote Exproler```が存在するため、それを押下する。  
```docker the_world_data```を右クリックし```Attach in New Window```を押下する。  
新規に開かれたVSCode(以下、開発VSCode)にて```Ctrl + K → O```と押下し、```/app/the-world-data```を開く

## npm run
開発VSCodeにて```Ctrl + J```を押下しターミナルを開き、```npm install```を実行する。  
続けて、```npm run```を実行し、アプリケーションを起動する。  
ブラウザにて```http://localhost:3000/```にアクセスし、画面が出たら終了。

