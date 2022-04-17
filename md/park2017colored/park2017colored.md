## Colored Point Cloud Registration Revisited--ICCV'17
[原文](../paper_pdf/Park_Colored_Point_Cloud_ICCV_2017_paper.pdf)
## 简介
传统ICP方法在很多情况下不能获得足够精确的配准结果，在加入颜色限制信息之后可以显著地提高精度。简单地方法是直接在xyzrgb的6D空间内进行匹配，但是这可能会搜寻到距离遥远但是颜色相似的点，因此会产生误差。本文在3D几何空间内搜寻匹配，将色彩信息引入到迭代中形成一种联合优化方法。作者定义了一个连续可微的光度测量方法，它的梯度指示颜色是如何随位置变化的。作者在每个点的切面上引入了一个虚拟图像，为隐性的颜色变化提供了一个局部近似。