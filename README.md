# Titanic: Machine Learning from Disaster

## 主要处理步骤:
1. 预处理：填补缺省值，从原column中提取信息成为新的数据栏
2. scale to normalize the data
4. create dummy variables to flip column and row
5. set appropriate para for the random forest model 

## 解题方法：
1. 刚开始不知道数据之间的关系，所以用表格，相关性检验，分类平均值等探索性方法确定数据之间的关系，比如
-  之前并不知道年纪，性别，舱位对生还有影响，需要作图来看
-  之前并不知道familysize对生还有影响，作图，以及分类二次处理
-  embark, fare 的缺省值究竟是多少，需要通过其他非缺省值部分计算
-  title, family size, ticket prefix 这些都是二次变量，这些变量的出现是基于探索性分析的结果

2. 在脑海中基本对这个模型比较确定的情况下，开始做模型处理。这中间涉及：
-  dummy variable
-  调整参数
-  scaling
-  套用不同模型比较留下预测最好的

## 说明：
<br>v1. 是分析阶段的代码草图</br>
v2. 是最后得出结果部分的代码