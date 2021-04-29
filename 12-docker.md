1. [基础教程](https://github.com/datawhalechina/team-learning-program/tree/master/Docker)

2. 添加个人用户

- sudo groupadd docker          #添加docker用户组
- sudo gpasswd -a $XXX docker   #检测当前用户是否已经在docker用户组中，其中XXX为用户名，例如我的: lyp
- sudo gpasswd -a $USER docker  #将当前用户添加至docker用户组
- newgrp docker                 #更新docker用户组

**以上**步骤运行完了，重启终端

配置过程中需要多长重启系统才能有效