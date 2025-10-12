# dotfiles

Collection of my `vim`, `zshell`, and `brew` configurations.

## Symlink

```bash
ln -s "$(pwd)/.vimrc" ~/.vimrc
```

## iTerm2

```bash
brew install iterm2
```

## Oh-my-zsh

```bash
brea install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

[omz Cheet Sheet](https://kapeli.com/cheat_sheets/Oh-My-Zsh_Git.docset/Contents/Resources/Documents/index)

- `g`
- `gp`
- `gcm`
  - I love this! Very useful!!!
- `gco`

```bash
# zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

# zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Brew Installs

```bash
brew install gh
brew install typos-cli
brew install mysql-client
brew install fzf
brew install tree
brew install kubecolor

# Development & Virtual Environments
brew install openssl@3
brew install pipx
brew install nvm
brew install rbenv
brew install direnv
brew install gradle
brew install pkc-config  # C/C++ linking tool

# Kubernetes
brew install k9s
brew install kubectx  # kubens도 포함됨
brew install kube-ps1  # CLI UI enhancement
brew install istioctl

# Docker
brew install colima
```

## Git

```bash
git config --global user.name "bluehorn07"
git config --global user.email "bluehornblues@gmail.com"
```

## Helm Plugins

- [helm-diff](https://github.com/databus23/helm-diff)

```bash
helm plugin install https://github.com/databus23/helm-diff
```

## Kubernetes Krew

https://krew.sigs.k8s.io/docs/user-guide/setup/install/

```bash
$ kubectl krew install view-secret
$ kubectl krew install df-pv
$ kubectl krew install neat
```

## Java

```bash
brew install openjdk@17
```

`gradle`, `java`까지 모두 설치됨. `$JAVA_HOME` 세팅 추가로 필요함.
그래야 vscode의 Java Extension에서 제대로 인식 가능함.


`~/.zshrc` 파일에 아래 내용 추가 해야 함.

```bash
# Java 17 (Homebrew)
export JAVA_HOME=/opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk/Contents/Home
export PATH="$JAVA_HOME/bin:$PATH"
```

그리고 `gradle.properties` 파일 생성해서 아래와 같이 작성

```ini
# Homebrew로 설치한 Java 17 경로를 명시적으로 지정
org.gradle.java.installations.paths=/opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk/Contents/Home
```

## AWS CLI

https://docs.aws.amazon.com/ko_kr/cli/latest/userguide/getting-started-install.html


## Mac Applications

- [Rectangle](https://rectangleapp.com/)
  - 윈도우 분할
- [Karabiner-Elements](https://karabiner-elements.pqrs.org/)
  - 키보드 매핑 커스텀
- [Clocker](https://github.com/n0shake/clocker)
  - 메뉴바에 세계 시간 표시
- [Rancher Desktop](https://rancherdesktop.io/)
  - 로컬에서 Kubernetes & Docker 환경 구축
- [Terminus](https://termius.com/)
  - SSH 접속 관리

## Keyboard

- Karabiner-Elements 세팅
- [원화(₩) 대신 백틱(`) 입력되게 하기](https://www.korecmblog.com/blog/backtick-fix)
