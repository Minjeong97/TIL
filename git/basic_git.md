# git-hub

## github 연결
```python
master가 떠 있는 지 확인.
samsung@DESKTOP-SK8P7M3 MINGW64 ~/TIL (master)

$ touch basic_git.md

$ git remote add origin https://github.com/Minjeong97/TIL.git

$ git add .

$ git commit -m 'first commit'

$ git log

$ git push -u origin master

크롬에 커넥션 창이 뜰 것.

samsung@DESKTOP-SK8P7M3 MINGW64 ~/TIL (master)
$ git push -u origin master
info: please complete authentication in your browser...
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1.37 KiB | 280.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0       
To https://github.com/Minjeong97/TIL.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

samsung@DESKTOP-SK8P7M3 MINGW64 ~/TIL (master)
```

## github 커밋 시, 가입 메일 주소 다를 경우
`git config --global user.email 'github가입@이메일'`

## 금일 사용한 명령어
git remote add <name> <URL>
git push <name> <branch>

    * push
    * pull
    * commit
    * clone = init

### clone
    1. git status
    2. git pusth origin master
    3. git add .
    4. git commit -m '1125 am'
    5. git push origin master
    6. cd
    7. cd Desktop/
    8. git clone `https://github.com/Minjeong97/TIL.git` (utl은 git-code-https)
    9. ls # 이제 desktop에 til 폴더가 clone됨.

### push
    1. touch test.txt
    2. git add . 
    3. git commit -m ‘add test.txt’ 
    4. git push origin master

### pull
    1. ls # 아직 커밋을 안해줘서 새로 생성된 파일이 없음
    2. git pull origin master
    3. ls # 이제 새로 생성된 파일 볼 수 있음.

### ex
1. test.txt 삭제
    `$ rm test.txt`
   * 주의: ②(remote) ③(desktop, 외부pc)에서 삭제하면 안됨


1. commit 추가
    `$ git add .`
    `$ git commit -m 'remove test.txt'`

2. remote에 반영
    `get push origin master`

3. desktop에 반영
    `$ git pull origin master`
    `$ ls`

4. 모든 sync 맞추기 

5. 이제 끝났으니, desktop에 만들어놓은 거 삭제
    `cd ..`
    `rm -rf TIL/`


### 기타
git log short
sync가 맞는 지 확인하는 명령어
`$ git log --oneline`


## 주의사항
1. 현재 위치를 잘 확인한다.
2. Repo 안에서 repo(= master)를 만들지 않는다.
   1. 이미 git init을 한 곳 안에
   2. 하위 폴더를 만들고 `$ mkdir test`
   3. 그 하위 폴더에서 `$ git init`을 하지 않는다.
   4. `master` 떠 있으면 init 제발 X !!!
3. Home(~)에서 init 하지 않는다.
    * Repo 안에서 repo(= master)를 만드는 셈.
4. (지금은) github에서 직접 수정하지 않는다.

## 권장사항
1. commit 메시지는 간결명료하게
2. 모든 repo (프로젝트)는
   1. README.md : README는 어떤 프로젝트에 대한 설명서
        `$ touch README.md`
        작성한 후,
        `$ git add README.md`
        `$ git commit -m 'add readme'`
        `$ git push origin master`
        ※ github README 에서 Add a README 버튼 누르지 않기
   2. .gitignore 를 담고 있어야 한다.