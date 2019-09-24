
`clone` 于 `git@github.com:Terry-Ye/docker-lnmpr.git` 

- 修复了一些问题。
- 升级php版本至7.1,mysql至5.7
- 支持laravel5.6环境

**使用方法**

 ```
    git clone https://github.com/DaemonWen/docker_lnmpr.git
    cd docker_lnmpr
    
    docker-compose up //构建镜像运行容器
   
 ```
  ------------------
  
 **2018.12.05 更新加上docker-sync**
 
 ***目的***
 -  解决mac文件系统跟docker之间文件系统格式转换导致缓慢的问题 详情见 https://docs.docker.com/docker-for-mac/osxfs/#mounts
 
 
 - 安装docker-sync
 ```
  gem install docker-sync
 brew install fswatch
 brew install unison
 brew install eugenmayer/dockersync/unox   //安装这一步，如果是mac较新的系统可能会出错，改成  brew install unox --with-python3 试试
 ```
 - docker-sync的配置可以参考  https://github.com/EugenMayer/docker-sync/wiki/2.-Configuration
 
 
 配置参考了:https://github.com/ninghao/nest 跟 https://ruby-china.org/topics/37289
 
 ***注意***
 如果不需要使用docker-sync，需要把.env 文件重命名为其他文件即可
 
 ------------------------
***2018-12-14***
升级mojave后docker-sync无法使用，重新安装docker-sync后又可以使用。并且安装eugenmayer/dockersync/unox也不需要指定python3了
 
 
