# Linux下nodejs以及相关包的安装方法

#!/bin/bash

    #nodejs-install

    cd /tmp

>wget http://192.168.17.43/soft/node-v4.3.1-linux-x64.tar.gz

    tar xf  node-v4.3.1-linux-x64.tar.gz

    cp -a node-v4.3.1-linux-x64 /usr/local/node

    ln -s /usr/local/node/bin/node /usr/bin/node

    ln -s /usr/local/node/bin/npm /usr/bin/npm

    node -v
    
    npm -v
    
    安装pm2
    
    npm set registry http://npm.hzins.com    ##修改npm源
    
    ln -s /usr/local/node/bin/pm2 /usr/bin/pm2
    
    npm install pm2 -g
    
    pm2 install pm2-logrotate
    
    安装gm包
    
    wget  http://192.168.17.43/soft/GraphicsMagick-1.3.24-1.el6.x86_64.rpm
    
    yum install GraphicsMagick-1.3.24-1.el6.x86_64.rpm -y