Experience:
[TrainingArguments](https://huggingface.co/transformers/main_classes/trainer.html?highlight=trainingarguments#transformers.TrainingArguments)
运行脚本：
建立一个 run.sh 文件，内容如下:
#!/bin/bash
python run_clm.py \
    --model_name_or_path gpt2 \   # 需要下载的预训练模型
    --dataset_name wikitext \     # 测试的数据集
    --dataset_config_name wikitext-2-raw-v1 \ # 数据集 config 名称
    --per_gpu_train_batch_size 1 \            # batch_size，默认为8
    --save_total_limit 1 \                    # 仅仅保存最优模型
    --do_train \                           
    --do_eval \ 
    --output_dir /tmp/test-clm               # 训练结果保存路径

    configuration 保存在 /tmp/test-clm/config.json
    model weights 保存在 /tmp/test-clm/pytorch_model.bin
