# KNN-research

## 研究不同KNN搜索算法在不同维度数据中的表现

我们对这三个数据集shuttle mnist ijcnn1进行预处理，转化为标准的表格格式进行测试。
手动实现KNN-brute-search，和使用sklearn实现KD-tree和Ball-tree，再上面的数据集中进行测试和比较
最后得出结论，对于KD-tree和Ball-tree，KD-tree在低纬度数据(小于20)中效果比Ball-tree好，而高纬度数据(大于700)正好相反，Ball-tree全方位优于KD-tree。
而手动实现的KNN-brute-search因为是纯python实现，所以会比底层使用c的sklearn库中的慢很多。
