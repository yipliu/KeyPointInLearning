@dataclass
class ModelArguments:
    """
    我们选择 从头训练 或者 fine-tune 的模型可设置参数
    """
    model_name_or_path: 
    权重初始化的 path
    从头训练时候不赋值

    model_type:
    如果是从头训练，输入 model_type, Transformers 中所包含的 Model 的名字

    config_name:
    预训练 config name 或者 path

    tokenizer_name:
    预训练 tokenizer name 或者 path

    cache_dir:
    存储预训练模型（从 huggingface.co 中下载下来的）


@dataclass
class DataTrainingArguments:
     """
     设置我们用于训练和评估模型的 数据参数
     """
    dataset_name:
    使用 dataset 的名字 

    dataset_config_name
    dataset 的 configuration name

    train_file:
     输入的 训练集，必须为 csv, json, txt 文件
    validation_file:
     
     block_size:
      设置模型最大的单个句子的长度
    preprocessing_num_workers:
    预处理所用 processes 的数量

[TrainingArguments](https://huggingface.co/transformers/main_classes/trainer.html?highlight=trainingarguments#transformers.TrainingArguments):
output_dir:  Model predictions 和 checkpoints 的保存路径

do_train
do_eval
do_predict

evaluation_strategy
 训练时所采取的 evaluation strategy:
 no: 训练时不采取 evaluation
 steps, eval_steps 时都采用 evaluation
 epoch: 每个 epocah 采用 evaluation

 prediction_loss_only 
 当执行 eval 和 predictions 只返回 loss

 per_device_train_batch_size 默认为 8 
 训练时候，每个 GPU 的 batch size

 per_device_eval_batch_size
 eval 时候， 每个 GPU 的batch size

 gradient_accumulation_steps 默认为 1

 learning_rate: 5e-5
 Adam 的 初始学习率
 weight_decay: 0
 

 num_train_epochs: 默认值为 3 
  training epochs 的总数
 max_steps: 默认值为 -1
  如果给正数，将会覆盖 num_train_epochs, 表示 the total number of training steps to perform

 logging_dir:
 tensorboard log 目录，默认为 
 current_datetime_hostname

 logging_steps 500, 两个 log 之间的 update steps
 save_steps 500 两个checkpoint 之间的 update steps
 save_total_limit: 是否删除前一个 checkpoints

 load_best_model_at_end: 默认 False
 在每个 training 后，是否选择保存 the best model
 如果设为 True，那么 save_steps 参数将会被忽略，模型将会在每个evalution选择最优的进行保存



