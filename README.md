# 学习笔记--LTspice

## 导入第三方库

>原则，高内聚，低耦合，建好的仿真模型发给别人，直接能用

首先复现这篇文章https://zhuanlan.zhihu.com/p/457648572

下载LM318的模型

在官网上下载spice模型
![Alt text](pictures/image-1.png)

下载下来解压缩，文件名叫"LM318.301"，不管它

可以用这个文件在LTspice中自动创建图标，但是这样搞就是一个方框，不像是运放
在建好的模型中把运放换成LM318
![Alt text](pictures/image-3.png)

运行，符合预期
![Alt text](pictures/image.png)

把include语句注释掉，直接把.301文件复制进仿真，结果也符合预期

![Alt text](pictures/image-2.png)
