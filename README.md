# dotfiles

Collection of my `vim`, `zshell`, and `brew` configurations.

## Symlink

```bash
ln -s "$(pwd)/.vimrc" ~/.vimrc
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
brew install kube_ps1  # CLI UI enhancement
brew install istioctl
```

## Kubernetes Krew

https://krew.sigs.k8s.io/docs/user-guide/setup/install/

```bash
$ kubectl krew
```


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
