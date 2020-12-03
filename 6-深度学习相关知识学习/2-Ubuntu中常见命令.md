1. export
shell 执行代码运行时候常见如下代码
```python
export TRAIN_FILE=/path/to/dataset/wiki.train.raw
export TEST_FILE=/path/to/dataset/wiki.test.raw

python run_language_modeling.py
```
export的作用告诉代码，TRAIN_FILE的位置在/path/to/dataset/wiki.train.raw