# 在DISABLE 浏览器GPU/METAL 加速的情况下，HLAB依然返回GPU模式的矩阵乘法更快。

这是天上掉馅饼了吗？

不是，

原因在于HHLAB的首席科学家， 核心数学库贡献者所写的HLAB的矩阵乘法的时间复杂度是NAIVE的N^3，而webGL的矩阵乘法是经过优化的正常的Strassen's Algorithm，在没有GPU的情况下，WebGL会Fall back to Strassen's Algorithm；自然比HHLAB自带的最差N^3算法好。。。

