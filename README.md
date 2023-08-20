# Mac 再インストール

## brew install
https://brew.sh/index_ja
```bash
$ xcode-select --install
$ sudo softwareupdate --install-rosetta
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
$ (echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> ~/.zprofile
$ eval "$(/opt/homebrew/bin/brew shellenv)"
```

### インストール
https://formulae.brew.sh/cask/
```
$ brew install php \
php@8.1 \
composer \
wget \
asdf \
ffmpeg \
tree \
coreutils \
curl \
awscli
```

### asdf の PATH を通す
https://asdf-vm.com/guide/getting-started.html
```
$ echo -e "\n. $(brew --prefix asdf)/libexec/asdf.sh" >> ${ZDOTDIR:-~}/.zshrc
$ source ~/.zshrc
```

### asdf - nodejs
```
asdf plugin add nodejs
asdf install nodejs latest
asdf global nodejs latest
corepack enable
asdf reshim nodejs
```

### asdf - php
```
asdf plugin add php
mkdir ~/.asdf/installs/php
ln -s /opt/homebrew/opt/php ~/.asdf/installs/php/8.2
ln -s /opt/homebrew/opt/php@8.1 ~/.asdf/installs/php/8.1
asdf reshim
asdf list php
asdf global php 8.2
```


### brew cask
```
$ brew install --cask docker \
google-chrome \
eset-cyber-security \
jetbrains-toolbox \
google-drive \
libreoffice \
expressvpn \
visual-studio-code \
keyboardcleantool \
epic-games \
adobe-creative-cloud \
google-japanese-ime \
geekbench \
karabiner-elements \
rambox \
logi-options-plus \
zoom \
libreoffice-language-pack --language=ja\
slack \
postman \
firefox \
path-finder \
microsoft-remote-desktop \
warp \
keka
```

Apple Store
  Brother iPrint&Scan（プリンタードライバーは別途WEBから）
  Brother P-Touch Editor
  magnet
  Nas Navigator 2

サイトインストール
- MyIP
https://www.interlink.or.jp/service/myip/
- iPrint&Scan Push Scan Tool
https://www.brother.com/apps/ps/ja/index.htm


# 設定
## JetBrains
	Appearance & Behavior > System Settings > Project
		Default project directory
## キーボード
	Karabinar キーボードJIS選択

	反応速度リピート速度
	$ defaults write -g InitialKeyRepeat -int 11
	$ defaults write -g KeyRepeat -int 1

## プリンター
	システム設定 > プリンタとスキャナ
