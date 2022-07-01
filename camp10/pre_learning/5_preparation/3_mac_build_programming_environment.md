# (Mac OS) 実習環境の構築 <!-- omit in toc -->
このセクションでは実習に必要なツールのインストール方法を説明します。

お使いのPCに以下のツールがインストールされていない場合は、ご用意をお願いします。
- [ターミナル](#ターミナル)
- [Homebrew](#homebrew)
- [C++ コンパイラ](#c-コンパイラ)
- [make](#make)
- [git/github](#gitgithub)
  - [git](#git)
  - [github](#github)
- [Zoom](#zoom)
- [テキストエディタ(任意)](#テキストエディタ任意)

※お使いの PC が会社のものである場合などで、事前にプロキシの設定が必要の場合は、ご自身で設定の上、進めて頂きますようお願い致します。
## ターミナル

**terminal.app** が標準搭載されているので、こちらを起動してください。

その他、これに相当するターミナルソフトであればご自身の使いやすいものを選択して頂いて構いません。

## Homebrew

Macで必要なツールやパッケージをインストールするために使用するものです。

インストールされているかの確認は以下のコマンドで行います。
インストールされている場合はバージョンなどが確認できます。

```sh
$ brew -v
----
Homebrew 3.2.5
Homebrew/homebrew-core (git revision c9729aea64; last commit 2021-07-31)
Homebrew/homebrew-cask (git revision 5b86d1b4f8; last commit 2021-07-30)
```
インストールされていない場合は以下を実行してください。

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

正常に Homebrew がインストールされたかどうかは以下のコマンドで確認して下さい。

```sh
brew doctor
```

##  C++ コンパイラ

C++を用いて開発を行うため、C++のコンパイラが必要です。

インストールされているかの確認は以下のコマンドで行います。
インストールされている場合はバージョンなどが確認できます。
```sh
g++ -v
----
Configured with: --prefix=/Library/Developer/CommandLineTools/usr --with-gxx-include-dir=/Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/include/c++/4.2.1
Apple clang version 11.0.3 (clang-1103.0.32.62)
Target: x86_64-apple-darwin19.6.0
Thread model: posix
InstalledDir: /Library/Developer/CommandLineTools/usr/bin
```

すでにMacにはコンパイラが標準で搭載されているはずですが、無い場合は以下のコマンドを実行して下さい。

```
brew install gcc
```

## make

C++プログラムをWebots上でビルドする際には**make**を必要とします。

インストールされているかの確認は以下のコマンドで行います。
インストールされている場合はバージョンなどが確認できます。

```sh
make -v
```

無い場合は以下のコマンドを実行してください。

```
brew install make
```

## git/github
LED-Camp10で使用するソースコードはgithubで共有します。
また、チームメンバとコードの共有を行う手段としてもお使い頂けます。

gitの操作に不慣れな方はGoogleDriveでも共有の場を設けますので、そちらをお使い頂くことも可能ですが、当日チームの方針によってはgitを使用する場合もあるかと思いますので、極力セットアップは行っておきましょう。

gitコマンドがあるかどうかの確認と、githubアカウントを用意します。

### git
以下のコマンドでgitコマンドが存在するか確認してください。

```sh
git --version
----
git version 2.24.3 (Apple Git-128)
```
無ければ以下を実行してください。

```
brew install git
```

※プロキシの設定が必要となるPCでは git クライアント(git コマンド)自体にも設定が必要となる場合がございます。この後の事前学習で git を使用しますが、プロキシの設定が解決できない場合でも代替手段をご紹介しますのでその際はそちらをご参考ください。

### github
すでに**github**アカウントをお持ちの方はスキップしてください。

githubアカウントをお持ちでない方は<a href="https://github.co.jp/" target="_blank" rel="noopener noreferrer">こちら</a>より、アカウントの作成(サインアップ)をお願い致します。無料のアカウントで十分です。

### 作成したgithubアカウントをローカルに設定する  <!-- omit in toc -->
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
当日の講義は **Zoom**を用いて行います。

<a href="https://zoom.us/download" target="_blank" rel="noopener noreferrer">こちら</a>より Mac 版の Zoom クライアントをダウンロードし、インストールをお願い致します。

当日はビデオ ON の状態にすることもありますので、**必ずスピーカ、マイク、カメラをご用意** の上、動作確認を事前に行って頂きますようお願い致します。

## テキストエディタ(任意)

基本的にテキストエディタがなくても実習は行っていただけますが、ソースコードを読む際にはテキストエディタがあると便利です。LED-Camp 実行委員も使用している **VSCode** を紹介致します。

<a href="https://code.visualstudio.com/" target="_blank" rel="noopener noreferrer">こちら</a>よりVSCodeのダウンロードページにジャンプしますので、画面に従ってダウンロードからインストールまで行ってください。

起動するには以下のコマンドをターミナルに打つと起動できます。

```sh
code
```

その他ご自身の使いやすいエディタがあればそちらをお使い頂いて構いません。
