### Git 명령어



```html
git init
```

: .git 하위 디렉토리 생성, 깃 초기화

```html
git add
```

: git add <파일명> 으로 working directory에서 staging area로 이동시켜줌.

여기서 staging area는 git add 명령어를 실행하여 커밋 전 파일들이 모인 공간  

 ```
 mkdir 파일이름
 ```

: 디렉토리 생성

```
rm -rf.git
```

: 숨겨진 git 삭제

```
git rm --cached 파일이름 
```

: 다시 untracked 된 상태로 돌아감 

```
git commit -m "커밋명"
```

:  커밋을 함으로써 어떤 작업을 했는지 알 수 있게끔 해준다. 단계별로 깃발을 꽂는 행위라고 볼 수 있음.

```
git log --oneline
git log --author="Nam"
git log --before="2023-01-22"
```

:로그를 한줄로 표현 (히스토리 출력)

```
git echo (파일) >> .gitignore
```

(파일)을 버전관리에서 제외시킴.

```
git diff
```

 Working Directory와 Staging Area 사이 차이를 보여줌

현재 디렉토리와 이전 커밋했을 때의 차이 확인할 때 사용

```
git diff --staged
```

커밋된 파일상태와 추가된 파일 상태 비교

이미 add 명령어로 인해 Staging area에 올라간 상황일때 사용