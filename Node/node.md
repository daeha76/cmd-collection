# nvm 설치
```sh
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```
그 후 환경 변수를 설정하고 프로파일 파일을 다시 로드합니다
```sh
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```
위 명령어를 쉘 프로파일 파일(~/.bashrc, ~/.bash_profile, ~/.zshrc 등)에 추가한 후 파일을 다시 로드합니다
```sh
source ~/.bashrc  # or source ~/.zshrc for zsh users
```

# Node.js 버전 설치
이제 원하는 Node.js 버전을 설치할 수 있습니다. 예를 들어, Node.js 16, 20, 22 버전을 설치하려면 다음 명령어를 사용합니다
```sh
nvm install 16
nvm install 20
nvm install 22
```
## 기본 Node.js 버전 설정
설치된 Node.js 버전 간에 전환하려면 `nvm use` 명령어를 사용
```sh
nvm use 16  # Node.js 16 버전 사용
nvm use 20  # Node.js 20 버전 사용
nvm use 22  # Node.js 22 버전 사용
```
특정 버전을 기본 버전으로 설정하려면 `nvm alias default` 명령어를 사용합니다
```sh
nvm alias default 20  # Node.js 20 버전을 기본으로 설정
```
## 설치된 Node.js 버전 목록 확인
설치된 Node.js 버전 목록을 확인하려면 `nvm ls` 명령어를 사용합니다
