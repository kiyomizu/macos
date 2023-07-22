# Mac 再インストール

- Chrome
- Google 日本語入力
- Docker
- Toolbox
- Adobe cc
- Logicool
- ESET
- GeekBench6
- Karabinar キーボードJIS対応
- Command Line Tools => Git
- Google Drive
- libreOffice
- Nas Navigator 2

## brew
	/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
	Next Steps の2行を実行
iPrint&Scan Push Scan Tool

Apple Store
	Brother iPrint&Scan（プリンタードライバーは別途WEBから）
	Brother P-Touch Editor
Adobe CC
Xcode (AppStore)
UnrealEngine5
Interlink VPN
Express VPN



# 設定
## JetBrains
	Appearance & Behavior > System Settings > Project
		Default project directory
## キーボード
	Karabinar キーボードJIS選択

	反応速度リピート速度
	$ defaults write -g InitialKeyRepeat -int 11
	$ defaults write -g KeyRepeat -int 1

## ユーザー追加
	pastime

## プリンター
	システム設定 > プリンタとスキャナ

## brew install
	brew install wrap
	brew install ffmpeg
	brew install --cask visual-studio-code
	brew install libreoffice-language-pack --language=ja
	brew install --cask rambox
	brew install --cask docker

## asdf 
	nodejs
		asdf plugin add nodejs
		asdf install nodejs latest
		asdf global nodejs latest
		corepack enable
		asdf reshim nodejs

## php
		brew install php
		brew install php@8.1
		asdf plugin add php
		mkdir ~/.asdf/installs/php
		ln -s /opt/homebrew/opt/php ~/.asdf/installs/php/8.2
		ln -s /opt/homebrew/opt/php@8.1 ~/.asdf/installs/php/8.1
		asdf reshim
		asdf list php
		asdf global php 8.2
		brew install composer
		brew install wget

zsh 関連
