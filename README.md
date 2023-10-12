# git 명령어 연습 23/10/12

practice git command
111
## [ex0] linux git 설정
```
1. git 설치
2. git config --global user.name [이름]
3. git config --global user.email [메일]
4. git init : git 저장소가 되길 원하는 폴더에서 입력
5. git remote add (remote repository의 이름) (원격 저장소 github URL)
   (https://발급받은 토큰 코드@github.com/저장소 상세 경로.git)
7. git pull origin main
8. git remote rm origin : remote 설정이 잘못 되어 있으면 삭제
```

## [ex1] 기본 동작
```
1. git clone (git 저장소 URL) / git pull
2. echo "Hello, Git!" > README.md
3. git add -A : 수정된 파일 전부를 스테이지 영역으로 추가
4. git status : 현재 스테이지 영역 확인
5. git commit -m "feat: README.md update"
6. git push (remote repository의 이름) (브랜치 이름)
7. git log
* 패스워드로 로그인은 21년 8월 13일 부터 불가능 => tocken 발급받아서 인증
```

## [ex2] 브랜치 기본 명령어
```
1. git branch (생성하려는 브랜치명) (분기해 나올 브랜치명)
2. git branch -m (기존 브랜치명) (새로운 브랜치명)
3. git checkout (이동하려는 브랜치명)
   git switch (이동하려는 브랜치명)
4. git checkout -b (생성하고 바로 이동하려는 브랜치명)
5. git branch -v : 현재 등록된 브랜치 확인
6. git branch --merged / git branch --no-merged

git branch -D (삭제하려는 브랜치명)
git push origin --delete (삭제하려는 브랜치명)
```

## [ex3] 브랜치 stash
```
- git stash : 브랜치 이동 시 commit 하지 않고 잠시 저장
1. echo "Hello, Git!" > README.md
2. git stash
```
