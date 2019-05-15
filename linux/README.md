# linux服务部署node项目
 ## 安装wget命令
    1. sudo apt-get install wget

 ## 安装node.js
    1.wget https://nodejs.org/dist/v10.9.0/node-v10.9.0-linux-x64.tar.xz

 ## 解压node.js并且copy 到/usr/local/下 且重新命名为nodejs
    1. tar xf node-v10.9.0-linux-x64.tar.xz -C /usr/local/
    2. cd /usr/local/
    3. mv node-v10.9.0-linux-x64/ nodejs

 ## 建立软连接方式，设置为全局
    1. sudo ln -s /usr/local/nodejs/bin/node /usr/local/bin
    2. sudo ln -s /usr/local/nodejs/bin/npm /usr/local/bin

 ## 安装淘宝镜像或者yarn,并且设置为全局
    1. npm install -g cnpm --registry=https://registry.npm.taobao.org
    2. sudo ln -s /usr/local/nodejs/bin/cnpm /usr/local/bin

 ## 安装PM2部署
    1. npm install pm2 -g
    2. sudo ln -s /usr/local/nodejs/bin/pm2 /usr/local/bin

 ## 安装lrzsz工具包
    1. yum install lrzsz
    2. sz file //上传文件夹

 ## 安装nginx 
    1. yum -y install make zlib zlib-devel gcc-c++ libtool  openssl openssl-devel

    2.