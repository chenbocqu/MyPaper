# SEMMDL Model

整体SEMMDL模型如下：

<img src="https://github.com/chenbocqu/MyPaper/blob/master/pic/semmdl_model.png" />

其中，L为SVM的优化目标，具体如下，

<img src="https://github.com/chenbocqu/MyPaper/blob/master/pic/SVM_obj.png" />

本文中采用二次Hinge-Loss（①经实验证明，效果会更好；②有解析解，效率更高）

<img src="https://github.com/chenbocqu/MyPaper/blob/master/pic/squared_hinge_loss.png" />

关于上述模型的求解，可以转化为如下3个子过程！

## Step 1. 低维空间字典学习

固定$P$和$<W,b>$，相当于求解如下模型

