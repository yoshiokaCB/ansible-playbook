# Mac用のansibleのplaybook

## Usage

ターミナルで実行
```
$ xcode-select --install
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew install caskroom/cask/brew-cask
$ brew update
$ brew install ansible
$ echo 'export HOMEBREW_CASK_OPTS="--appdir=/Applications"' >> ~/.bash_profile
$ mkdir ~/.provisioning && cd $_
$ git clone https://github.com/yoshiokaCB/ansible-playbook.git
```

ansibleの実行
```
$ ansible-playbook -i hosts -vv ~/.provisioning/ansible-playbook/general.yml
```
