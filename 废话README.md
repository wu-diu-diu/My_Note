# Nonsense_sentence_classifier
## 模型
模型基于huggingface上的开源模型：`bert-base-chinese`，使用huggingface提供的微调大模型的方法，利用自制的废话文学数据集进行微调
## 废话文学数据集
- 废话主要搜集自中文互联网，如百度，知乎上面的废话合集约300条左右。
- 利用GPT生成相同格式的废话大概700条左右。
- 正常语料来源于huggingface上的中文数据集。
- 可用于文本分类等任务的验证。

本项目只是个人的一个小尝试，没有涉及任何微调技巧，全是标准流程。
