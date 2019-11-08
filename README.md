# BERT 对多标签文本分类
调用bert-base-uncased的pytorch预训练模型做对一个多标签文本做分类


文件夹下包含子文件夹，其中data是我们文本存储文件夹，包含训练、验证和测试的数据。
对数据的描述：每个实例包含一句话和它所对应的标签，标签总共包含16个。具体标签内容在data文件夹下的label.txt文件中。
首先我们需要下载transformer包，利用pip install transformer或者conda命令即可安装。
然后我们需要打开run_glue.py文件，修改文件路径，将文本文件夹路径（data_dir）、模型（bert_base_uncased）路径进行修改。其中模型路径包含三部分内容，第一部分是uncased-model.bin,也就是pytorch版本模型路径。第二部分是模型所对应的json配置文件路径。第三部分就是vocab.txt路径，需要一一在run_glue.py进行修改。

模型相关的三个文件需要自己下载！
debug  run_glue.py文件 MODEL_ALL中包含三个文件的下载地址！
