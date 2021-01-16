实验室的Ubuntu服务器往往是很多同学一起使用，因此我们要实习如下几个功能
- 多人使用 ==> 个人账户
   - Ubuntu上创建自己的[账户]((http://note.youdao.com/noteshare?id=509ebb3d2a673114114b62bfbce246f8))
- 远程控制 ==> 安装 X2GO
   - 服务器上安装[X2GO Server](https://wiki.x2go.org/doku.php/doc:installation:x2goserver)
   - 服务器上安装XFCE4作为服务器的虚拟化桌面："sudo apt-get install xfce4"
   - 在本地安装[X2GO Client](http://ithelp.physics.ucdavis.edu/kb/x2go)
   - 在Client登录时候，登录界面要与你安装的(XFCE)一致
  
- 远程传输文件 ==> 安装 FileZilla
  - Windows 下安装[客户端](https://zhuanlan.zhihu.com/p/35846871)
  - Ubuntun安装[openssh-server](https://blog.csdn.net/baidu_38505667/article/details/103029510?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.control&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.control)

- Chorme 浏览器下载插件 => XDM
   - XDM使用[教程](https://zhuanlan.zhihu.com/p/37941433) 
   - 记得设置代理

