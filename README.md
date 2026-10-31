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
PS C:\Users\User\desktop\ttoli54\hi> docker info
Client:
 Version:    29.9.2
 Context:    desktop-linux
 Debug Mode: false
 Plugins:
  agent: Docker AI Agent Runner (Docker Inc.)
    Version:  v1.152.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-agent.exe
  ai: Docker AI Agent - Ask Gordon (Docker Inc.)
    Version:  v1.33.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-ai.exe
  buildx: Docker Buildx (Docker Inc.)
    Version:  v0.38.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-buildx.exe
  compose: Docker Compose (Docker Inc.)
    Version:  v5.6.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-compose.exe
  debug: Get a shell into any image or container (Docker Inc.)
    Version:  0.49.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-debug.exe
  desktop: Docker Desktop commands (Docker Inc.)
    Version:  4.97.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-desktop.exe
  dhi: CLI for managing Docker Hardened Images (Docker Inc.)
    Version:  v0.0.9
    Path:     C:\Program Files\Docker\cli-plugins\docker-dhi.exe
  extension: Manages Docker extensions (Docker Inc.)
    Version:  v0.2.32
    Path:     C:\Program Files\Docker\cli-plugins\docker-extension.exe
  init: Creates Docker-related starter files for your project (Docker Inc.)
    Version:  v1.4.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-init.exe
  mcp: Docker MCP Plugin (Docker Inc.)
    Version:  v0.44.2
    Path:     C:\Program Files\Docker\cli-plugins\docker-mcp.exe
  model: Docker Model Runner (Docker Inc.)
    Version:  v1.2.9
    Path:     C:\Program Files\Docker\cli-plugins\docker-model.exe
  offload: Docker Offload (Docker Inc.)
    Version:  v0.7.21
    Path:     C:\Program Files\Docker\cli-plugins\docker-offload.exe
  pass: Docker Pass Secrets Manager Plugin (beta) (Docker Inc.)
    Version:  v0.3.2
    Path:     C:\Program Files\Docker\cli-plugins\docker-pass.exe
  sandbox: "docker sandbox" is deprecated, use Docker Sandboxes instead (Docker Inc.)
    Version:  v0.13.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-sandbox.exe
  scout: Docker Scout (Docker Inc.)
    Version:  v1.27.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-scout.exe

Server:
 Containers: 2
  Running: 1
  Paused: 0
  Stopped: 1
 Images: 2
 Server Version: 29.9.2
 Storage Driver: overlayfs
  driver-type: io.containerd.snapshotter.v1
 Logging Driver: local
 Cgroup Driver: cgroupfs
 Cgroup Version: 2
 Plugins:
  Volume: local
  Network: bridge host ipvlan macvlan null overlay
  Log: awslogs fluentd gcplogs gelf journald json-file local splunk syslog
 CDI spec directories:
  /etc/cdi
  /var/run/cdi
 Discovered Devices:
  cdi: docker.com/gpu=webgpu
 Swarm: inactive
 Runtimes: io.containerd.runc.v2 runc
 Default Runtime: runc
 Init Binary: docker-init
 containerd version: b7a25261e029d68978bbf290df0a62fc819b3c51
 runc version: v1.5.2-0-g29dd3dc2
 init version: de40ad0
 Security Options:
  seccomp
   Profile: builtin
  cgroupns
 Kernel Version: 7.0.14-linuxkit
 Operating System: Docker Desktop
 OSType: linux
 Architecture: x86_64
 CPUs: 8
 Total Memory: 1.916GiB
 Name: docker-desktop
 ID: ca431dfc-87ae-45ae-ae41-5348d3646e36
 Docker Root Dir: /var/lib/docker
 Debug Mode: false
 HTTP Proxy: http.docker.internal:3128
 HTTPS Proxy: http.docker.internal:3128
 No Proxy: hubproxy.docker.internal
 Labels:
  com.docker.desktop.address=npipe://\\.\pipe\docker_cli
 Experimental: false
 Insecure Registries:
  hubproxy.docker.internal:5555
  127.0.0.0/8
  ::1/128
 Live Restore Enabled: false
 Firewall Backend: iptables

PS C:\Users\User\desktop\ttoli54\hi> docker images
                                                    i Info →   U  In Use
IMAGE                ID             DISK USAGE   CONTENT SIZE   EXTRA
hello-world:latest   c567b231f656       25.9kB         9.49kB    U
ubuntu:latest        6a06111c3b0a        163MB         45.9MB    U
PS C:\Users\User\desktop\ttoli54\hi> docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED       STATUS       PORTS     NAMES
48701143dfea   ubuntu    "bash"    8 hours ago   Up 8 hours             serene_jepsen
PS C:\Users\User\desktop\ttoli54\hi> docker ps -a
CONTAINER ID   IMAGE         COMMAND    CREATED       STATUS                   PORTS     NAMES
48701143dfea   ubuntu        "bash"     8 hours ago   Up 8 hours                         serene_jepsen
fb2ce77d2778   hello-world   "/hello"   8 hours ago   Exited (0) 8 hours ago             friendly_blackburn
PS C:\Users\User\desktop\ttoli54\hi>
```
