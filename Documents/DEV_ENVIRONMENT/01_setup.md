# 開発環境構築手順
## 概要
当システム開発では、DockerとVSCodeを使用して開発を実施していく。  
これの目的として、開発者間での環境相違をなくすこと、開発者間同士でDocker x VSCodeを用いた環境での開発手法の知識を深める目的である。

## Docker環境の構築
Dockerは主に使用されている以下のOS全てで使用可能である。
Docker環境構築方法についてはDocker社が提供しているドキュメントに従い構築するものとする。  
※なお、WindowsにおいてはDocker Desktopを使用するように記載しているが、パフォーマンスが悪い場合があるので、その場合はWSL2内にLinuxをインストールしその中でDocker Engineを動かす方法でも可。  
* Windows
  * https://docs.docker.com/desktop/install/windows-install/
* Linux
  * https://docs.docker.com/engine/install/
* macOS
  * https://docs.docker.com/desktop/install/mac-install/

## VSCode環境の構築
Visual Studio Code(以下VSCode)はMicrosoftが提供しているエディタである。  
エディタではあるが、拡張機能の導入や設定ファイル等を記載することにより、VSCode上でアプリケーションのデバッグ・編集中のコードの補完が実施することが可能となっている。  
### インストール
公式サイト(https://code.visualstudio.com/download)にアクセスし、各々環境に合うものをDLしインストールする。

### 拡張機能のインストール
以下の拡張機能をインストールする
* Docker
  * Docker関連のコマンドをVSCode上で完結させるもの。ファイルを右クリックでやりたいことができる。
  * https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker
* Dev Containers
  * Docker上で動いている開発環境にVSCodeで乗り込むもの。
  * https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers