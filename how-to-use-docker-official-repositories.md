# 如何使用 Docker 官方镜像

为了更好地推广 Docker 开源技术，方便国内的开发者使用 Docker 官方的镜像，[docker.cn](https://docker.cn) 每日将 Docker 官方镜像仓库的最新版本同步到国内的服务器。

无需注册 [docker.cn](https://docker.cn) 的帐号，用户即可使用 Docker 官方的镜像。 Docker 官方镜像是指保存在 [Docker Hub](https://registry.hub.docker.com) 的 [stackbrew](https://registry.hub.docker.com/repos/stackbrew/) 用户下的所有镜像仓库。这些镜像有些是 Docker 官方制作的，有些是由这些软件的官方社区维护的。

### 方法 1.

如果使用 `docker pull` 命令下载官方镜像仓库，如下载 ubuntu 的官方镜像仓库，将 `docker pull ubuntu` 中的 `ubuntu` 替换为 [docker.cn](https://docker.cn) 的 docker 用户下的同名仓库即可，即 `docker pull docker.cn/docker/ubuntu` 。

以下是当前同步的所有镜像列表：

```
docker pull docker.cn/docker/hello-world
docker pull docker.cn/docker/rails
docker pull docker.cn/docker/ruby
docker pull docker.cn/docker/nginx
docker pull docker.cn/docker/hylang
docker pull docker.cn/docker/crate
docker pull docker.cn/docker/php
docker pull docker.cn/docker/mongo
docker pull docker.cn/docker/zend-php
docker pull docker.cn/docker/wordpress
docker pull docker.cn/docker/ubuntu-upstart
docker pull docker.cn/docker/ubuntu-debootstrap
docker pull docker.cn/docker/ubuntu
docker pull docker.cn/docker/registry
docker pull docker.cn/docker/redis
docker pull docker.cn/docker/python
docker pull docker.cn/docker/postgres
docker pull docker.cn/docker/perl
docker pull docker.cn/docker/opensuse
docker pull docker.cn/docker/node
docker pull docker.cn/docker/neurdebian
docker pull docker.cn/docker/mysql
docker pull docker.cn/docker/mageia
docker pull docker.cn/docker/jruby
docker pull docker.cn/docker/jenkins
docker pull docker.cn/docker/java
docker pull docker.cn/docker/hipache
docker pull docker.cn/docker/golang
docker pull docker.cn/docker/gcc
docker pull docker.cn/docker/fedora
docker pull docker.cn/docker/docker-dev
docker pull docker.cn/docker/debian
docker pull docker.cn/docker/crux
docker pull docker.cn/docker/clojure
docker pull docker.cn/docker/cirros
docker pull docker.cn/docker/centos
docker pull docker.cn/docker/busybox
docker pull docker.cn/docker/buldpack-deps
```

### 方法 2.

如果使用 `Dockerfile` 的方式，请替换 `FROM` 的镜像仓库名称即可，如将：

```
FROM ubuntu:14.04.1
```

替换为

```
FROM docker.cn/docker/ubuntu:14.04.1
```


> 我们还会将更多的存储在 [Docker Hub](https://registry.hub.docker.com) 的优秀镜像同步到国内服务器上，方便国内的开发者使用。请关注我们的微博帐号**[Docker 中文社区](http://www.weibo.com/dockboard)**，获取最新的消息。
