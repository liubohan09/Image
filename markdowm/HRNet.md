# HRNet

1.2d检测方法

2.单一个体输出目标

3.如果，先检测每个人框，再检测每个关键点

基于回归的方式，直接预测关键点位置坐标

基于heatmap的方式，即针对每个关键点预测一张热力图

![1663811542440](C:\Users\ADMINI~1\AppData\Local\Temp\1663811542440.png)

关键点的热力图，score最大的位置

损失预测

MSE，LABEL是2d高斯分布 ，每个关键点计算的是用的不同权重

Obeject keypoints similarity

![1663812689133](C:\Users\ADMINI~1\AppData\Local\Temp\1663812689133.png)

![1663812799146](C:\Users\ADMINI~1\AppData\Local\Temp\1663812799146.png)

keep ratio 输入高宽比不变

