# Docker

## 核心概念解析

- **Client**： Docker客户端（ docker ）是许多Docker用户与Docker交互的主要方式。当您使用诸如之类的命令  
    时 docker run ，客户端会将这些命令发送到 dockerd ，以执行这些命令。该 docker 命令使用Docker  
      
    API。Docker客户端可以与多个守护程序通信。  
    
- **守护程序**：Docker守护程序（ dockerd ）侦听Docker API请求并管理Docker对象，例如图像，容器，网络和  
    卷。守护程序还可以与其他守护程序通信以管理Docker服务。  
      
    Docker对象  
    - **镜像**：是创建容器的模板，里面会有一些基础的环境，比如ubuntu/alpine等；
    - **容器**：是运行的镜像，提供统一且一致的运行环境。默认情况下，容器与其他容器及其主机之间的隔离  
        度相对较高。您可以控制容器的网络，存储或其他底层子系统与其他容器或与主机的隔离程度。  
        
- **仓库**：Docker仓库存储Docker映像。Docker Hub是任何人都可以使用的公共仓库，并且默认情况下， Docker已配置为在Docker Hub上查找映像。您甚至可以运行自己的私人仓库，比如：harbor。

## 运行步骤

`docker run` 命令  
以下命令运行一个 ubuntu 容器，以交互方式附加到本地命令行会话，然后运行 /bin/bash 。  
  
当运行此命令时：  
`docker run -i -t ubuntu /bin/bash`

1. 如果在 ubuntu 本地没有该映像，则Docker会将其从Hub仓库（默认）中下载，如果已经下载（docker pull  
    ubuntu）则会跳过；  
    
2. Docker会创建一个新容器。
3. Docker将一个读写文件系统分配给容器，作为其最后一层。这允许运行中的容器在其本地文件系统中创建或  
    修改文件和目录。  
    
4. Docker创建了一个网络接口，默认没有指定任何网络选项时，将容器连接到默认网络，包括为容器分配新网  
    段的IP地址。默认情况下，容器可以使用主机的网络连接连接到外部网络。  
    
5. Docker启动容器并执行 /bin/bash 。由于容器是交互式运行的，并且已附加到的终端（由于 -i 和 -t 标  
    志），可以在输出记录到终端时使用键盘提供输入。  
    
6. 当键入 exit 以终止 /bin/bash 命令时，容器将停止但不会被删除，可以重新启动（docker start）或删除它  
    (docker rm)。  
    

## Docker-compose

Docker Compose是一款旨在帮助定义和共享多容器应用程序的工具，使用Compose，可以通过创建一个YAML文  
件来定义容器服务，并且可以使用类似于Docker的命令将所有内容进行管理（比如，启动、停止、重新部署等）。  

```Plain
# Use root/example as user/password credentials
version: '3.1'
services:
    db:
    image: mysql
    # NOTE: use of "mysql_native_password" is not recommended:
    <https://dev.mysql.com/doc/refman/8.0/en/upgrading-from-previous-series.html\#upgrade->
    caching-sha2-password
    # (this is just an example, not intended to be a production configuration)
    command: --default-authentication-plugin=mysql_native_password
    restart: always
    environment:
        MYSQL_ROOT_PASSWORD: example
    adminer:
        image: adminer
        restart: always
        ports:
            - 8080:8080
```

等价于

```Plain
docker run --restart=always -e MYSQL_ROOT_PASSWORD=example -d mysql:tag --default-
authentication-plugin=mysql_native_password

docker run --restart=always -p 8080:8080 adminer
```

配置好 `docker-compose.yml` 文件后，执行下面命令运行在后台，可在 docker 客户端查看

```Plain
docker-compose up -d
```

TODO: mysql 默认密码为 example

docker ps 查看进程

## client

- docker build
- docker pull
- docker run

## docker host

### 镜像

images

### 容器

containers

## docker registry

模版

## 运行

docker