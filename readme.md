# Bert 微调示例
这是一个bert预训练模型调整为文本二分类任务的实例，如果需要多分类的教程，请看https://mccormickml.com/2019/07/22/BERT-fine-tuning/
## 下载预训练模型
从官网下载模型
https://huggingface.co/bert-base-chinese
至少下载其中的config.json  pytorch_model.bin  tokenizer.json  vocab.txt这四个文件
## 调整数据集大小和平衡
训练集总共7000多条数据 5000正样本
应将正负样本平衡
而且实际上bert只需要200多条数据就可以很好的拟合，所以将数据集缩小到适合自己设备大小可以有效缩减训练用时，这里留给你们自己调整
