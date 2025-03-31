Linux, Mac のみです。（Windows は Ubuntu 内に構築することを前提）

# インストール直後に実行する内容
https://github.com/kiyomizu/macos

# 言語パッケージマネージャー

## asdf
https://asdf-vm.com/

### asdf インストール
```sh
$ brew update
$ brew upgrade
$ brew install asdf
```

### asdf アップデート
xcode ライセンス規約承認
```sh
$ sudo xcodebuild -license accept
# brew, asdf アップデート
$ brew update && brew upgrade asdf
$ asdf plugin update --all
$ asdf list 
```

## aqua
https://aquaproj.github.io/

## mise
https://mise.jdx.dev/


# 開発言語
## nodejs
```sh
$ asdf plugin add nodejs
$ asdf plugin add yarn
$ asdf install nodejs latest
$ asdf install yarn latest
$ asdf global nodejs latest
$ asdf global yarn latest
```

## php インストール
```sh
$ brew install postgresql
$ asdf plugin add php
$ asdf list all php
$ asdf install php 7.4.29
$ asdf install php 8.1.5
$ asdf reshim php

// 全体は7.4.29。特定ディレクトリのみ8.1.5 の場合
$ asdf global php 7.4.29
$ php -v
> PHP 7.4.29 (cli) (built: Apr 20 2022 17:18:17) ( NTS )
Copyright (c) The PHP Group
Zend Engine v3.4.0, Copyright (c) Zend Technologies

$ mkdir php8 && cd !$ && asdf local php 8.1.5 && php -v
> PHP 8.1.5 (cli) (built: Apr 20 2022 17:32:15) (NTS)
Copyright (c) The PHP Group
Zend Engine v4.1.5, Copyright (c) Zend Technologies
```

## rust インストール
```sh
$ asdf plugin-add rust
$ asdf install rust latest
$ asdf reshim rust
$ asdf global rust 1.15.0
$ cargo -V
> cargo 1.60.0 (d1fd9fe2c 2022-03-01)
```

## python
```sh
$ asdf plugin-add python
$ asdf install python latest
$ asdf reshim python
$ asdf global python 3.10.4
$ python -V
> Python 3.10.4
```

## golang
```sh
$ asdf plugin-add golang
$ asdf install golang latest
$ asdf reshim golang
$ asdf global golang 1.18.1
$ go version
> go version go1.18.1 darwin/amd64
```

# AI
https://cloud.signate.jp/column/list-of-generation-ai-types

## クラウドLLM

[chatgpt](https://openai.com/)

[gemini](https://gemini.google.com/)

[grok](https://x.ai/)

[claude](https://claude.ai/)

[Cline](https://github.com/cline/cline)

[cursor](https://www.cursor.com/ja)

## ローカルLLM

## 記事生成

## コード生成

## 画像生成

## 動画生成

## 音楽生成

## 3D生成


# デザイン

## Figma

## 
