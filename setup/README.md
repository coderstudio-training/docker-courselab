# Set Up Docker and Git

Docker runs as a background service on server operating systems, but in a local environment the easiest option is Docker Desktop.

We'll also use [Git](https://git-scm.com) for source control, so you'll need a client on your machine to talk to GitHub.

## Git Client - Mac, Windows or Linux

Git is a free, open source tool for source control:

- [Install Git](https://git-scm.com/downloads)

## Docker Desktop - Mac or Windows

If you're on macOS or Windows 10, Docker Desktop is for you:

- [Install Docker Desktop](https://www.docker.com/products/docker-desktop)

The download and install takes a few minutes. When it's done, run the _Docker_ app and you'll see the Docker whale logo in your taskbar (Windows) or menu bar (macOS).

> On Windows 10 the install may need a restart before you get here.

## **OR** Docker Engine - Linux

<details>
  <summary>Running Docker on Linux</summary>

Docker Engine is the background service which runs containers. You can install it - along with the Docker command line - for lots of different Linux distros:

 - [Install Docker Engine](https://docs.docker.com/engine/install/)
 - [Install Docker Compose](https://docs.docker.com/compose/install/)

> If you're using WSL2 on Windows 10/11, it's much easier to use Docker Desktop which integrates with your WSL distro.

For more info: https://docs.docker.com/desktop/wsl/
</details><br />

## **OR** Docker Install Script (Recommended)

Running this one-liner script on Mac, Linux, Windows (WSL 2):
  ```
  curl -fsSL https://get.docker.com | sh
  ```


## Check your setup

When you have Git and Docker installed you should be able to run these commands and get some output:

```
git --version
```

I'm using Git for Linux and my output is:

```
git version 2.34.1
```

Then run:

```
docker version
```

I'm using Docker on Linux and mine says:

```
Client: Docker Engine - Community
 Version:           26.0.0
 API version:       1.45
 Go version:        go1.21.8
 Git commit:        2ae903e
 Built:             Wed Mar 20 15:17:48 2024
 OS/Arch:           linux/amd64
 Context:           default

Server: Docker Engine - Community
 Engine:
  Version:          26.0.0
  API version:      1.45 (minimum version 1.24)
  Go version:       go1.21.8
  Git commit:       8b79278
  Built:            Wed Mar 20 15:17:48 2024
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          1.6.28
  GitCommit:        ae07eda36dd25f8a1b98dfbf587313b99c0190bb
 runc:
  Version:          1.1.12
  GitCommit:        v1.1.12-0-g51d5e94
 docker-init:
  Version:          0.19.0
  GitCommit:        de40ad0
```

And then:

```
docker compose version
```

My output is:

```
Docker Compose version v2.25.0
```

> Your details and version numbers may be different - that's fine. If you get errors then we need to look into it, because you'll need to have Docker running for all of the exercises.

> ❗ If you're running Docker Desktop on Windows, make sure you're in _Linux container mode_. This is the default mode, but if you've changed to using Windows containers (from the whale toolbar menu), then you'll need to switch back.