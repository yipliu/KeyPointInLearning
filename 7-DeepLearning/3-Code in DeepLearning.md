rnn = getattr(nn, rnn_type): rnn_type: LSTM, GRU
==> nn.LSTM or  nn.GRU

# 多个文件中函数导入问题
问题描述：
在一个工程中，我们想导入自己在这个工程其他文件中写的函数或者类
解决方法：
sys.path.append(project_path)

ROOT_DIR = os.path.abspath("")


# Pip 安装 requirements.txt
pip install --upgrade pip
pip install -r requirements.txt
pip install -U nltk 安装最新版本的 nltk/ 也可以更新用