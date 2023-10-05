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
```powershell
> mkdir            //directory 만들기
> rm -r            //directory 삭제(하위 포함)
```
```powershell
> exit 터미널 종료
```
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
```powershell
> git branch AAAA   // AAAA브랜치 만들기
```
```powershell
> git switch AAAA   // AAAA브랜치로 전환
```
```powershell
> git remote add origin <git 주소>    // git 주소 와 연결
```
```powershell
> git remote -v     // git 연결상태 보여줌
```
