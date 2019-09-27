# 聚类算法的应用及比较
## 数据集
本次实验采用了两个数据集，分别是digit手写字数据集和document文本数据集，这两个数据集都集成在了SkLearn中
### digit数据集
* 调用方法
  > `sklearn.datasets.load_digits()`
* 数据示例
  > ![示例数据](pic/digit_sample.jpg)
### document数据集
* 调用方法
  >`sklearn.datasets.fetch_20newsgroups()`
* 数据示例
  > ![示例数据](pic/doc_sample.jpg)
## 手写字数据集上的各算法的比较
### 实验运行结果
![运行结果](pic/result_digit.jpg)
### 可视化
对数据中的每张图片，进行PCA进行降维<br>                  
![结果图](pic/digit.jpg)
## 文本数据集上的个算法的比较
由于该数据集有20类样本，如果考虑20类样本的话，数据过多，聚类的时间会较慢，而且也不便于可视化，所以此次选取了数据集中的4类样本来进行聚类
### 运行结果
![运行结果](pic/result_doc.jpg)
### 可视化
对于数据汇总中的每个文本，用svd进行降维<br>
![结果图](pic/document.jpg)
## 各类聚类算法比较
### Kmeans算法
*    KMeans算法又名k均值算法。其算法的思想大致为：先从样本中选取k个样本作为簇中心，并计算所有样本与当前“簇中心”的距离，对于每一个样本，将其划分到与其距离最近的“簇中心”所在的簇中，对于新的簇计算各个簇的的新的“簇中心”。
*    根据上述描述，我们可以概括KMeans算法的三个要点<br>
    1. 簇个数k的选择<br>
    2. 各个样本到“簇中心”的距离<br>
    3. 根据新划分的簇，更新“簇中心”
### AffinityPropagation相似传播算法
### MeanShift算法
### SpectralClustering算法
### Ward hierarchical clustering算法
### AgglomerativeClustering算法
### DBSCAN算法
### Gaussian Mixtures 算法
