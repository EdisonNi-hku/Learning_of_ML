# PCA and related algorithms
## 1. PCA
### 1.1. [基本原理](https://blog.csdn.net/program_developer/article/details/80632779)
将n维特征映射到k维上，这k维是全新的正交特征也被称为主成分，是在原有n维特征的基础上重新构造出来的k维特征。<br>

思考：我们如何得到这些包含最大差异性的主成分方向呢？

答案：事实上，通过计算数据矩阵的协方差矩阵，然后得到协方差矩阵的特征值特征向量，选择特征值最大(即方差最大)的k个特征所对应的特征向量组成的矩阵。这样就可以将数据矩阵转换到新的空间当中，实现数据特征的降维。<br>
![PCA](./pictures/PCA.PNG)<br>
[数学原理](http://blog.codinglabs.org/articles/pca-tutorial.html)