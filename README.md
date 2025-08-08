# DP-SAM

# 论文已经正式发表，随后即将公布代码
# The paper has been officially published, and then the code will be released.
https://cjig.cn/zh/article/doi/10.11834/jig.240540/
# 支持数据集
[Potsdam](https://github.com/Jacky-Android/pytorch_remote_sensing_segmentation?tab=readme-ov-file#potsdam)

[Vaihingen](https://github.com/Jacky-Android/pytorch_remote_sensing_segmentation?tab=readme-ov-file#vaihingen)

# 数据集准备

## Potsdam
数据集为城市区域的遥感影像语义分割数据集，特征影像数据分辨率为8米，包括38幅遥感影像，波段为红色、绿色，近红外波段，DSM波段，其中24幅完全标注，标注的土地覆盖类别包括：耕地：[0, 255, 255]，林地：[255, 0, 0]，草地：[0, 255, 0]，建筑用地：[255, 0, 255]，水域：[0, 0, 255]，未利用地及其他：[255, 255, 0])。数据详情：[http://www2.isprs.org/commissions/comm3/wg4/2d-sem-label-potsdam.html](http://www2.isprs.org/commissions/comm3/wg4/2d-sem-label-potsdam.html)

因为Potsdam数据集有38块，可以选择块来做为训练集，剩下的做为测试集
也可以使用我切好的
https://www.123pan.com/s/YnBgjv-D8j1H.html提取码:pots

https://drive.google.com/file/d/1NWLLVlUVaIZYwePbPx7Ca60AdyW-cdMT/view?usp=sharing

## Vaihingen
数据集包含33幅不同大小的遥感图像，每幅图像都是从一个更大的顶层正射影像图片提取的，图像选择的过程避免了出现没有数据的情况。顶层影像和DSM的空间分辨率为9 cm。遥感图像格式为8位TIFF文件，由近红外、红色和绿色3个波段组成。DSM是单波段的TIFF文件，灰度等级（对应于DSM高度）为32位浮点值编码。

切割好的数据集：
123盘：https://www.123pan.com/s/YnBgjv-rST4H.html提取码:Vsb8

Google Dirver:https://drive.google.com/file/d/1L2rxAzMm-pEV2dY111285t04hOm2L1hv/view?usp=drive_link

# 引用：

刘思涌， 赵毅力. 2025. 微调SAM的遥感图像高效语义分割模型DP-SAM. 中国图象图形学报， 30(8):2884-2896 DOI： 10.11834/jig.240540. 

Liu Siyong， Zhao Yili. 2025. DP-SAM： efficient semantic segmentation of remote sensing images by fine-tuning SAM. Journal of Image and Graphics， 30(8):2884-2896 DOI： 10.11834/jig.240540.

# 鸣谢
[GeoSeg](https://github.com/WangLibo1995/GeoSeg)

[Timm](https://github.com/huggingface/pytorch-image-models)

[pytorch](https://github.com/pytorch/pytorch)

[Albumentations](https://github.com/albumentations-team/albumentations)
