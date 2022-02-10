### このrepositoryについて

この新しいブログは[hugo](https://gohugo.io/)によって生成されたhtml/cssファイルにより構成されています。
詳しい仕組みは知らないので、ブログの記事にでもしてください。

### Hugoのインストール

> READ THE FUCKING MANUAL!!!!

まずは[公式のドキュメント](https://gohugo.io/getting-started/installing/)を読んでください。
読めたらそのままインストールしていいよ。
だめだったら↓を参照してください。

- windows

   まじで一ミリもわからん。*追記求む*。  
   よく見るパッケージマネージャーは`Chocolatey`。
   [Chocolatey](https://chocolatey.org/)

- Mac

   多分`homebrew`とかのパッケージマネージャーを使えばいいと思う。  
   [homebrewのページ](https://brew.sh/)

   一応コマンドを書いておく。
   ```
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   brew install hugo
   ```
   パッケージマネージャアンチとかなら↓のバイナリを生成する方法を使えばいいと思う。

- Linux

   `debian`系だと`snap`を使えばいい。
   すなわち、
   ```
   snap install hugo
   ```
   ただしバージョンが古かったりするので、ビルドしたいときもある。
   そのときは以下のようにビルドしよう。

- ビルドしたい！

   Goを入れる。(Goのインストール方法)[https://go.dev/doc/install]。
  - Mac
      `pkg`の解凍方法を忘れた。*追記求む*

      その後に
      ```
      export PATH=$PATH:/usr/local/go/bin >> ~/.zshrc
      ```
      とかを打てばよろしい。
  - Linux
      適当に`apt`とかでいれるとよろしい。
      あるいは`dpkg`して。
      さすがに`pacman`とかでも提供しているのではないか？
  - ビルド
  ```
    mkdir $HOME/src
    cd $HOME/src
    git clone https://github.com/gohugoio/hugo.git
    cd hugo
    go install --tags extended
  ```
  ここの`extended`フラグがないと動かないテーマとかもあるので`extended`推奨。

### Gitの使い方とか

*要追記。*(ここで書くことではないので文とかで誘導すればいい？)

### ブログの見方

`git`が使えるようになっているのが前提になっちゃう。すまぬ。

1. 手元にリポジトリを`clone`する。
   
   ```
   git clone https://github.com/RICORA/blog.git
   ```
   をコマンドラインとかなんかで入力する。

   そうすると今いるディレクトリの下に`blog`というディレクトリができる。

2. テーマを拾ってくる。
   
   `hugo`ではテーマを簡単に変更することができる。  
   このブログで使っているのは[hugo-theme-stack](https://github.com/CaiJimmy/hugo-theme-stack)なので、`blog/themes`ディレクトリに移動して、
   ```
   git clone https://github.com/CaiJimmy/hugo-theme-stack.git 
   ```
   を入力する。

3. ローカルサーバーを建てる。

   ```
   hugo server
   ```
   を入力する。
   好きなブラウザ（まあ中身は基本２種類しかないんだけど）に表示されているリンク（普通は`localhost:8080`)を入力すると、現状のままのブログが見れるはず。  
   良かったですね。
   
### ブログの書き方

1. ブランチを切る。

   ```
   git checkout -b (ブログに関するブランチ名)
   ```
   確認は
   ```
   git branch
   ```
   `master`で書いて`master`をぶっ壊しマスターしないようにしよう。

2. マークダウンファイルを生成する

   とりあえず、`blog`ディレクトリ直下で記事のファイル名を決めて
   ```
   hugo new content/posts/(ファイルの名前).md
   ```
   と打つ。

3. マークダウンファイルを編集する。

   好きなテキストエディタを使ってそのファイルを編集する。
   [マークダウンのお作法](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)にしたがって書けば、段落とか箇条書きとかができる。これが日本語版でないのは日本語で出てくるやつが表現のすべてをカバーしておらず、段落とかを書くときに困っちゃうため。     
   終わったらセーブしておく。

4. ローカル鯖を建てて確認する。

   さっきも書いたけど
   ```
   hugo server
   ```
   で`https://localhost:1313/blog`にアクセスすれば見れる。
   `127.0.0.1:1313/blog`でもよい。

5. commit && push
   
   しようね。

6. Pull Requestをつくる。

   以下はGitHub cliの場合。多分webページからでも同じことができるはず。
   ```
   gh pr create
   ```
   詳細を書いて、提出する。レビュワーが`accept`したら現時点だと`master`にマージされる。  
   ちゃんと適宜`pull`をしてコンフリクトさせないようにしましょう。

   おわり。よかったですね。
