1. Ubuntu 20.04 配置DL开发环境[教程](https://gist.github.com/amir-saniyan/b3d8e06145a8569c0d0e030af6d60bea)
2. [修改](https://blog.csdn.net/qq_33656324/article/details/94552156)Ubuntu下 jupyter notebook 工作目录
3. 配置 Anaconda 国内源：[清华源官网教程](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/),[矩池云](https://github.com/matpool/matools)


# Jupyter notebook 配置
1. 每创建一个Env后都需要做以下步骤才能让Jupyter使用conda的Env
   - 在虚拟环境下操作

    "pip install ipykernel"

2. 将虚拟环境与Jupyter连接

" python -m ipykernel install --user --name=env_name（虚拟环境的名字）"


# Ubuntu 修改 hosts
sudo vim etc/hosts
在 [ip网](https://site.ip138.com/raw.Githubusercontent.com/) 查询相应网站ip输入即可

3. VScode 基础[教程](https://www.bilibili.com/video/BV14U4y1p7LF)
- 创建.gitignore 文件，里面写入忽略的文件夹名称