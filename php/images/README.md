**FROM** 指定哪个镜像作为你的基础镜像，我们是以官方的php:7.4-fpm作为基础镜像

**ENV** 用于配置环境变量，在其他指令中可以直接引用ENV设置的环境变量

**RUN** 执行命令并创建新的Image Layer，看起来就跟shell命令一样

**WORKDIR** 指定工作目录，如果使用docker exec进入容器时，默认目录就是指定的工作目录，如/data


制作镜像命令：
 
 docker build -f Dockerfile.swoole -t hwphp:7.4.2 .

 docker build -f Dockerfile.swoole.cli -t phpswoole .

