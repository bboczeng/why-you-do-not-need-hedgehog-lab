# 在DISABLE 浏览器GPU/METAL 加速的情况下

HLAB 却可以显示你依然存在GPU加速。。。。

原因在于HLAB的矩阵乘法是N^3，而webGL的矩阵乘法是经过优化的正常的Strassen's Algorithm，在没有GPU的情况下，WebGL会Fall back to Strassen's Algorithm；自然比HHLAB自带的最差N^3算法好。

