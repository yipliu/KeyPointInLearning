1. 每创建一个Env后都需要做以下步骤才能让Jupyter使用conda的Env
   - 在虚拟环境下操作

    "pip install ipykernel"

2. 将虚拟环境与Jupyter连接

" python -m ipykernel install --user --name=env_name（虚拟环境的名字）
" 