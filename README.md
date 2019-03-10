# Arbitrary-Style-Transfer-Based-On-GAN
任意的图像风格迁移算法指同时输入一张自然图像C跟一张风格参照图像I,输出的图像O同时保存自然图像C的结构内容，同时也增加了风格图像I的风格信息。
由于GAN的判别器一般通过比较真实图像跟生成图像的真实程度，但图像风格迁移任务是没有真实的图像的，因此，算法通过将图像的风格信息以及结构内容信息进行重新再编码，实现了基于GAN的任意图像的风格迁移算法。

**Environment:**
- python 3.6
- pytorch 0.4.1
- ubuntu 16.04

**Test on Image:**
```
python testimage.py --content content_image --style style_image --output output_image
```
**Test on Video:**
```
python testvideo.py --content contentvideo.mp4 --style style_image/style_video 
```

**Results**
<img src="images/content/in1.jpg" width="200" hspace="5"><img src="images/style/in1.jpg" width="200" hspace="5"><img src="images/content/in3.jpg" width="200" hspace="5"><img src="images/style/in3.jpg" width="200" hspace="5">

<img src="samples/in1.jpg" width="400" hspace="10"><img src="samples/in3.jpg" width="400" hspace="10">

<img src="images/content/in2.jpg" width="200" hspace="5"><img src="images/style/in2.jpg" width="200" hspace="5"><img src="images/content/in4.jpg" width="200" hspace="5"><img src="images/style/in4.jpg" width="200" hspace="5">

<img src="samples/in2.jpg" width="400" hspace="10"><img src="samples/in4.jpg" width="400" hspace="10">

**References**
- [Learning Linear Transformations for Fast Arbitrary Style Transfer](https://arxiv.org/abs/1808.04537v1)
  Xueting Li, Sifei Liu, Jan Kautz, Ming-Hsuan Yang
- [Universal Style Transfer via Feature Transforms](https://arxiv.org/abs/1705.08086)
  Yijun Li, Chen Fang, Jimei Yang, Zhaowen Wang, Xin Lu, Ming-Hsuan Yang
