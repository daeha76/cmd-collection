# Git 커맨드 명령어 정리

## Git Bash 명령어
```powershell
> pwd
// print working directory : 현재 폴더 path를 보여줌
```

```powershell
> ls 
// 내부 폴더, 파일을 보여줌
> ls -a           //숨김파일까지 모두
> ls -l           //상세정보
> ls -r           //정렬순서를 거꾸로
> ls -t           //시간순으로 정렬
```

```powershell
> clear
```

```bash
> mkdir            //directory 만들기
> rm -r            //directory 삭제(하위 포함)
> rm -rf           //directory 삭제(하위 포함)
rm: 파일이나 폴더를 삭제하는 명령어입니다.
-r: 재귀적으로 삭제합니다. (하위 폴더와 파일을 모두 삭제)
-f: 강제로 삭제합니다. (삭제 확인을 묻지 않음)
```
```powershell
> Remove-Item -Path "C:\path\to\folder" -Recurse -Force
```

```powershell
> exit 터미널 종료
```

### push 하기
```powershell
> git add .
> git commit -m "설명"
or
> git commit -am "설명"

> git push -u origin <branch명>
```

```powershell
> git diff          //변경사항 확인하기
```

### 브랜치
```powershell
> git branch -a     // 모든 브랜치 보기
> git branch <AAAA>   // <AAAA> 브랜치 만들기
> git switch <AAAA>   // <AAAA> 브랜치로 전환
```

### Rebase 사용하기
```powershell
> git checkout <작업한 브랜치>   // 작업한 브랜치로 변경
> git rebase <대상 브랜치>       // 합칠 브랜치의 최신 상태로 리베이스합니다.
> git checkout <대상 브랜치>     // 합칠 브랜치로 변경
> git merge <작업한 브랜치>      // 작업한 브랜치를 합칠 브랜치로 머지
```

```powershell
> git remote add origin <git 주소>    // git 주소 와 연결
```

```powershell
> git remote -v     // git 연결상태 보여줌
```

```powershell
> git log --stat    // log 기록, "Q" : 빠져나오기
```
