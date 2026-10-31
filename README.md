# 나의 첫 번째 저장소

\# Dev Workspace 학습 일지



\## 2026.10.30 - Git \& GitHub 첫걸음



\### 오늘 배운 것

\- PowerShell 기본 명령어 (cd, ls, mkdir)

\- Git 저장소 만들기 (git init)

\- 커밋하기 (git add → git commit)

\- GitHub에 올리기 (git remote → git push)



\### 기억할 핵심 리듬

1\. git add .

2\. git commit -m "메시지"

3\. git push


\### 명령어 수행 실습

```
C:\Users\User> cd deskto

PS C:\Users\User\desktop> cd ttoli54

PS C:\Users\User\desktop\ttoli54> cd..

PS C:\Users\User\desktop> cd ~

PS C:\Users\User>

 C:\Users\User> cd desktop
PS C:\Users\User\desktop> cd ttoli54
PS C:\Users\User\desktop\ttoli54> ls

    디렉터리: C:\Users\User\desktop\ttoli54

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-10-31  오후 12:10                docker
d-----      2026-10-31   오후 4:23                terminal
d-----      2026-10-31   오후 4:27                terminal2
-a----      2026-10-31   오후 2:35            227 git 명령어.txt

PS C:\Users\User\desktop\ttoli54>

PS C:\Users\User\desktop\ttoli54> mkdir hi

    디렉터리: C:\Users\User\desktop\ttoli54

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-10-31   오후 4:51                hi

PS C:\Users\User\desktop\ttoli54> ls

    디렉터리: C:\Users\User\desktop\ttoli54

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2026-10-31  오후 12:10                docker
d-----      2026-10-31   오후 4:51                hi
d-----      2026-10-31   오후 4:23                terminal
d-----      2026-10-31   오후 4:27                terminal2
-a----      2026-10-31   오후 2:35            227 git 명령어.txt

PS C:\Users\User\desktop\ttoli54>

 C:\Users\User\desktop\ttoli54> cd hi
PS C:\Users\User\desktop\ttoli54\hi> ls
PS C:\Users\User\desktop\ttoli54\hi> new-item hello.txt

    디렉터리: C:\Users\User\desktop\ttoli54\hi

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----      2026-10-31   오후 4:56              0 hello.txt

 C:\Users\User\desktop\ttoli54\hi> set-content hello.txt "어렵지만 열심히!"
PS C:\Users\User\desktop\ttoli54\hi> get-content hello.txt
어렵지만 열심히!
PS C:\Users\User\desktop\ttoli54\hi>

PS C:\Users\User\desktop\ttoli54\hi> copy-item hello.txt hello-copy.txt
PS C:\Users\User\desktop\ttoli54\hi> ls

    디렉터리: C:\Users\User\desktop\ttoli54\hi

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----      2026-10-31   오후 5:02             18 hello-copy.txt
-a----      2026-10-31   오후 5:02             18 hello.txt

PS C:\Users\User\desktop\ttoli54\hi> move-item hello-copy.txt backup.txt

PS C:\Users\User\desktop\ttoli54\hi> ls

    디렉터리: C:\Users\User\desktop\ttoli54\hi

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----      2026-10-31   오후 5:02             18 backup.txt
-a----      2026-10-31   오후 5:02             18 hello.txt

PS C:\Users\User\desktop\ttoli54\hi> git init
Initialized empty Git repository in C:/Users/User/Desktop/ttoli54/hi/.git/
PS C:\Users\User\desktop\ttoli54\hi> git add

```
