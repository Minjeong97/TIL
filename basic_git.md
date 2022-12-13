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
