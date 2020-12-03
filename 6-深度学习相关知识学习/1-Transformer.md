Transformers 研究以下问题：
- 情感分析：分析一个文本是 Positive 还是
- 文本生成：
- Name entity recognition: 识别 Sentence 中 Entity 的类别(Person, plance,etc)
- Question answering:
- Filling masked text: given a text with masked words
  >e.g.: replaced by [MASK], fill the blanks
- Summarization: 给一段话生成一个 Summary
- Translation: 翻译
- Feature extracion: 返回一个文本的 Tensor


1. 可以在 [Model hub](https://huggingface.co/models) 上搜索到不同的预训练模型
2. [task summary](https://huggingface.co/transformers/task_summary.html) tutorial summarizes which class is used for which task
3. 在[Quick tour](https://huggingface.co/transformers/quicktour.html)的第二个例子中，会遇见ipywidgets没有安装：
   conda install -n base -c conda-forge widgetsnbextension
   conda install -n env_name -c conda-forge ipywidgets