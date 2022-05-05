# No Hedgehog Lab: 全网最好，不需要你懂得任何编程和计算机知识的，GPU 加速Python安装5分钟教程
**只用5分钟，服务一万年**

下面花5分钟介绍正确在本地安装GPU加速的Python，以及让您安装完后的第一分钟就可以书写您最爱的Python代码并且随时看到运行结果的办法。

## 好消息，这绝对不需要您懂得任何命令行或者计算机的知识。您不需要是计算机专业的学生，本教程最合适的，恰恰是商学院等有数据处理需求的学生们。当然前提还是有的，就是你要有一台电脑并且拥有一个互联网浏览器。对了，请确保您的电脑有电。

- **第一步**，打开<https://www.python.org/downloads/>下载符合您电脑操作系统类型的最新版的Python

小提示：这一步和您安装任何游戏、杀毒软件和黄色网站直播app一样，打开双击安装即可。我相信应该难不倒你吧？

![](imgs/Python下载.png)

预计花费时间：1分钟

- **第二步**，打开<https://www.jetbrains.com/pycharm/download>下载全球最好用最稳定最一致的Python所见即所得可视化IDE编程工具，让你摆脱对命令行和PIP的依赖（与困扰）

![](imgs/Pycharm下载.png)

预计花费时间：2分钟

小提示：这个工具有详细的提示；但最重要的是，他不需要你学会任何操作就能运行你的第一个python文件，他会自动默认选择您刚才安装好的python最新版作为python的interpreter（您不需要知道这是什么东西），在默认的main.py 中输入**1+1**，点击绿色的运行按钮，你就能看到**2**了。

- **第三步**，用全新免洗面免脑全球最强深度学习，矩阵运算，GPU加速库Pytorch安装方法

![](imgs/Pytorch下载.png)

打开<https://pytorch.org/get-started/locally/>，选择您的操作系统(Windows），再选择PIP，再选择Python，最后再选择CUDA 11.3即可。这样最后的结果是：

    pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113

复制如下代码到您最新打开的main.py中，点击绿色按钮运行，即可安装

![](imgs/Pycharm代码.png)

```py
import os

os.system('pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu113')
```

- **最后一步**，最后一步，运行下列代码证明自己的Pytorch和CUDA已经正确完整的安装成功啦！

```py
import torch

print(torch.cuda.is_available())
```

最后的结果应该是

![](最终结果.png)

```py
True
```
