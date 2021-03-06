# Depth Completion via Inductive Fusion of Planar LIDAR and Monocular Camera

## Paper

[Preprint](http://arxiv.org/abs/2009.01875)

## Abstract

Modern high-definition LIDAR is expensive for commercial autonomous driving vehicles and small indoor robots. An affordable solution to this problem is fusion of planar LIDAR with RGB images to provide a similar level of perception capability. Even though state-of-the-art methods provide approaches to predict depth information from limited sensor input, they are usually a simple concatenation of sparse LIDAR features and dense RGB features through an end-to-end fusion architecture. In this paper, we introduce an inductive late-fusion block which better fuses different sensor modalities inspired by a probability model. The proposed demonstration and aggregation network propagates the mixed context and depth features to the prediction network and serves as a prior knowledge of the depth completion. This late-fusion block uses the dense context features to guide the depth prediction based on demonstrations by sparse depth features. %
In addition to evaluating the proposed method on benchmark depth completion datasets including NYUDepthV2 and KITTI, we also test the proposed method on a simulated planar LIDAR dataset. Our method shows promising results compared to previous approaches on both the benchmark datasets and simulated dataset with various 3D densities.

## Network OverView
Detailed architecture of proposed inductive late-fusion network. The red and blue blocks indicate the context feature extraction network and depth feature extraction network. The corresponding Residual Block (RB) and Residual UpProjection Block (ReUpProj) are shown in the green blocks. The proposed inductive late-fusion block is shown in the yellow blocks.
![Network Architecture](network.png)

### Acknowledgments

This work was supported by the CMU Argo AI Center for Autonomous Vehicle Research.
