# LDA-SVM

- 使用LDA+SVM进行文本的分类
- 使用TF-IDF 表示文本的缺点：
```
     1. 没有考虑文本中词的词序信息（也就是语义）。
     2. 2. 会出现数据稀疏的情况
```
- 我采用文本的隐含主题，构造文本的向量表示，避免了文本向量表示数据稀疏的问题。实验的准确度能够达到 87%
- 数据集是搜狗新闻文本，想要数据集的可以添加我的 **qq：2590193099**

```
文件的说明：
	1.topic 文件夹是不同主题维数的矩阵的pickle存储
	2.tmp 是语料库的经过处理后的存储路径
	3.best_params.json是每个主题的最优化参数的存储
	4.pickle 每个人名的目标标签的存储
	5.param_result 文件夹是不同主题维数的和调参的结果存储
	6.tag是原始的语料库的文件
	7.preprocess是原始文件经过处理后（去掉数字和合并标题和content等操作）的文件存储路径
```