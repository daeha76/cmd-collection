# SSH 키를 사용하여 인증
1. SSH 키 생성

```sh
ssh-keygen -t rsa -b 4096 -C "daeha76@github.com"
```

2. SSH 에이전트 시작 및 키 추가

```sh
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

3. SSH 공개 키 복사

```sh
cat ~/.ssh/id_rsa.pub
```
출력된 공개 키를 복사

4. GitHub에 SSH 키 추가
 - GitHub 웹사이트에 로그인하고, 오른쪽 상단 프로필 사진을 클릭한 후 Settings 클릭
 - 왼쪽 메뉴에서 SSH and GPG keys를 클릭하고 New SSH key를 클릭
 - 제목과 복사한 공개 키를 붙여넣고 Add SSH key를 클릭

5. 리포지토리 클론

```sh
git clone git@github.com:{경로(https://제외)}
```
