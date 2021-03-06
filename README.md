# H2V

Code for TMM paper "Horizontal-to-Vertical Video Conversion"

<div align=center><img src="fig/motivation.png" width="500" /></div>

> [**Horizontal-to-Vertical Video Conversion**](https://arxiv.org/abs/2101.04051)            
> Tun Zhu, Daoxin Zhang, Yao Hu, Tianran Wang, Xiaolong Jiang, Jianke Zhu, Jiawei Li            
>  *IEEE Transactions on Multimedia (2021)*

## Abstract
At this blooming age of social media and mobile platform, mass consumers are migrating from horizontal video to vertical contents delivered on hand-held devices. Accordingly, revitalizing the exposure of horizontal video becomes vital and urgent, which is hereby settled, for the first time, with our automated horizontal-to-vertical (abbreviated as H2V) video conversion framework. Essentially, the H2V framework performs subject-preserving video cropping instantiated in the proposed Rank-SS module. Rank-SS incorporates object detection to discover candidate subjects, from which we select the primary subject to preserve leveraging location, appearance, and salient cues in a convolutional neural network. Besides converting horizontal videos to vertically by cropping around the selected subject, automatic shot detection and multi-object tracking are also integrated in the H2V framework to accommodate long and complex videos. For the development of H2V systems, we collect an H2V-142K dataset containing 125 videos (132K frames) and 9,500 cover images annotated with primary subject bounding boxes. On H2V-142K and public object detection datasets, our method demonstrates superior subject selection accuracy comparing to related solutions. Beyond that, our H2V framework is also industrially deployed hosting millions of daily active users and exhibits favorable H2V conversion performance. By making this dataset as well as our approach publicly available, we wish to pave the way for more horizontal-to-vertical video conversion solutions.

## News
* (2021.06) Accept by TMM

## Ranking-based Subject Setection (RankSS)

Code details (to appear)

![](fig/ss.png)

## Dataset
* H2V-142K can be downloaded from Alibaba Tianchi [official website](https://tianchi.aliyun.com/dataset/dataDetail?dataId=93339). Please find details there.

## Demo 

![](fig/result.png)

Visualization of results in the MSCOCO 2017 Val dataset , proposed H2V-142K dataset, and ASR dataset. The original input and final 9:16 frame output are on either side of the picture. It worth noticing that the horizontal target frame can be a different value such as 1:1, 3:4, etc. As the primary subject selected, our H2V framework is able to generate multiply outputs with different sizes simultaneously.

## Acknowledgement

The project is supported by Computer Vision and Video Analysis Lab of [AZFT](https://azft.alibaba.com/lab/?id=1)

## Citation

```
@article{zhu2021h2v,
  title={Horizontal-to-Vertical Video Conversion},
  author=Tun Zhu, Daoxin Zhang, Yao Hu, Tianran Wang, Xiaolong Jiang, Jianke Zhu and Jiawei Li},
  journal={arXiv preprint arXiv:2101.04051},
  year={2021}
}
```
