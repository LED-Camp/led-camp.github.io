# (Windows) 実習環境の構築 <!-- omit in toc -->
このセクションでは実習に必要なツールのインストール方法を説明します。

お使いのPCに以下のツールがインストールされていない場合は、ご用意をお願いします。


- [git/github](#gitgithub)
  - [git for Windows](#git-for-windows)
  - [github](#github)
- [Zoom](#zoom)
- [Discord](#discord)
- [テキストエディタ(任意)](#テキストエディタ任意)

※お使いの PC が会社のものである場合などで、事前にプロキシの設定が必要の場合は、ご自身で設定の上、進めて頂きますようお願い致します。\
※お使いの PC が会社のものである場合、会社によっては使用可能ソフトウェアに制限がある場合があります。ご自身で確認の上、ツールのインストールを進めて頂きますようお願い致します。

## git/github
LED-Camp10 で使用するソースコードは **github** で共有します。
また、チームメンバとコードの共有を行う手段としてもお使い頂けます。
gitの操作に不慣れな方は GoogleDrive でも共有の場を設けますので、そちらをお使い頂くことも可能ですが、当日チームの方針によっては git を使用する場合もあるかと思いますので、極力セットアップは行っておきましょう。

### git for Windows
既にお使いの**git**クライアントがあればスキップしてください。

1. <a href="http://git-scm.com/" target="_blank" rel="noopener noreferrer">こちら</a>より、**git for windows** のインストーラをダウンロードします。
    <p><img src="./imgs/git_for_windows_download.png"/></p>
2. インストーラを起動し、画面に従いインストールを進めます。
    - 全てデフォルトのまま next を押してください。
3. インストールが完了したら、**Git Bash** を起動するとターミナルエミュレータが開きます。この上でgitコマンドが使えるようになります。

※プロキシの設定が必要となるPCでは git クライアント(git for Windows)自体にも設定が必要となる場合がございます。この後の事前学習で git を使用しますが、プロキシの設定が解決できない場合でも代替手段をご紹介しますのでその際はそちらをご参考ください。

### github
すでに**github**アカウントをお持ちの方はスキップしてください。

githubアカウントをお持ちでない方は<a href="https://github.co.jp/" target="_blank" rel="noopener noreferrer">こちら</a>より、アカウントの作成(サインアップ)をお願い致します。無料のアカウントで十分です。

### 作成したgithubアカウントをgit for Windowsに登録する <!-- omit in toc -->
gitコマンドにgithubアカウントを設定しておきましょう。

```
git config --global user.name [Your User Name]
git config --global user.email [Your Email]
```

以下は例になります。
```
ex)
git config --global user.name sho-hama
git config --global user.name xxx@gmail.com
```

## Zoom
最終日のSWEST参加セッションは**Zoom**を用いて行います。

<a href="https://zoom.us/download" target="_blank" rel="noopener noreferrer">こちら</a>より Windows 版の Zoomクライアント をダウンロードし、インストールをお願い致します。

当日はビデオONの状態にすることもありますので、**必ずスピーカ、マイク、カメラをご用意** の上、動作確認を事前に行って頂きますようお願い致します。

## Discord
主にLED-Camp10前日までのコミュニケーションツールとして使用します。

<a href="https://discord.com/download" target="_blank" rel="noopener noreferrer">こちら</a>よりWindows 版の Discordクライアント をダウンロードし、インストールをお願い致します。

参加者同士や実行委員の交流、事前学習や環境構築のフォローの場として活用します。

## テキストエディタ(任意)
基本的にテキストエディタがなくても実習は行っていただけますが、ソースコードを読む際にはテキストエディタがあると便利です。LED-Camp 実行委員も使用している **VSCode** を紹介致します。

<a href="https://code.visualstudio.com/" target="_blank" rel="noopener noreferrer">こちら</a>よりVSCodeのダウンロードページにジャンプしますので、画面に従ってダウンロードからインストールまで行ってください。

ご自身の使いやすいエディタがあればそちらをお使い頂いて構いません。
