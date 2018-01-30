[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

# Optical Flow Algorithm Resources
A curated list of resources dedicated to optical flow algorithms. Any suggestions and pull requests are welcome.

## Papers & Code

### Classical methods
- [1981-IJCAI, Lucas-Kanade method] An iterative image registration technique with an application to stereo vision
- [1981-AI, Horn-Schunck method] Determining optical flow [`paper`](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.66.562&rep=rep1&type=pdf)
- [2004-ECCV, Brox method] High Accuracy Optical Flow Estimation Based on a Theory for Warping [`paper`](http://www.mia.uni-saarland.de/Publications/brox-eccv04-of.pdf) [`code`](https://docs.opencv.org/master/d7/d18/classcv_1_1cuda_1_1BroxOpticalFlow.html)
- [2005-IJCV] Lucas/Kanade meets Horn/Schunck: Combining local and global optic flow methods [`paper`](http://www.mia.uni-saarland.de/Publications/bruhn-ijcv05c.pdf)
- [2007-DAGM, TVL1 method] A duality based approach for realtime tv-l1 optical flow [`paper`](A duality based approach for realtime tv-l1 optical flow) [`code`](https://docs.opencv.org/master/d6/d39/classcv_1_1cuda_1_1OpticalFlowDual__TVL1.html)
- [2011-TPAMI, LDOF flow] Large displacement optical flow: descriptor matching in variational motion estimation [`paper`](https://lmb.informatik.uni-freiburg.de/people/brox/pub/brox_tpami10_ldof.pdf) [`code`](https://lmb.informatik.uni-freiburg.de/resources/binaries/)

### Deep learning based methods
- [2015-ICCV, FlowNet1] FlowNet: Learning Optical Flow with Convolutional Networks [`paper`](https://arxiv.org/abs/1504.06852) [`new code`](https://github.com/liruoteng/FlowNet)  [`old code`](https://lmb.informatik.uni-freiburg.de/resources/software.php)
- [2017-CVPR, FlowNet2] FlowNet 2.0: Evolution of Optical Flow Estimation with Deep Networks [`paper`](https://arxiv.org/abs/1612.01925) [`code`](https://github.com/lmb-freiburg/flownet2) [`homepage`](https://lmb.informatik.uni-freiburg.de/Publications/2017/IMKDB17/)

### Optical flow in severe environment (haze, rain)
- [2017-Xiv] Robust Optical Flow Estimation in Rainy Scenes [`paper`](https://arxiv.org/pdf/1704.05239.pdf)

### Others
- [2010-ECCV] Dense point trajectories by GPU-accelerated large displacement optical flow [`paper`](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2010/EECS-2010-104.pdf) [`code`](https://lmb.informatik.uni-freiburg.de/resources/binaries/)

### Optical flow toolkit
- [Li Routeng's toolbox] Python-based optical flow toolkit for existing popular dataset [`code`](https://github.com/liruoteng/OpticalFlowToolkit)

## Datasets
- [`Middlebury`](http://vision.middlebury.edu/flow/) `2009`
  - 8 image pairs for training, with ground truth flows generated using four different techniques
  - Displacements are very small, typi- cally below 10 pixels.
- [`KITTI`](http://www.cvlibs.net/datasets/kitti/) `2012` [`paper`](http://www.cvlibs.net/publications/Geiger2013IJRR.pdf)
  - 194 training image pairs, large displacements, contains only a very special motion type
  - The ground truth is obtained from real world scenes by simultaneously recording the scenes with a camera and a 3D laser scanner.
  - Task: stereo, flow, sceneflow, depth, odometry, object, road, tracking, semantics, etc.
- [`MPI Sintel`](http://sintel.is.tue.mpg.de/) `2012` [`paper`](http://files.is.tue.mpg.de/black/papers/ButlerECCV2012-corrected.pdf)
 - 1041 training image pairs, ground truth from rendered artificial scenes with special attention to realistic image properties
 - Task: optical flow.
- [`Flying Chairs (Vision group, Uni-Freiburg)`](https://lmb.informatik.uni-freiburg.de/resources/datasets/FlyingChairs.en.html) `2015`
  - 22872 image pairs, a synthetic dataset with optical flow ground truth
  - Task: optical flow.
- [`ChairsSDHom (Vision group, Uni-Freiburg)`](https://lmb.informatik.uni-freiburg.de/resources/datasets/FlyingChairs.en.html) `2017`
  - Task: optical flow
  - Designed to be robust to untextured regions and to produce flow magnitude histograms close to those of the UCF101 dataset (small displacement, less than 1 pixel).

## Open source implementation
- [Optical Flow with OpenCV 3](https://docs.opencv.org/master/d7/d3f/group__cudaoptflow.html) [Extra modules](https://docs.opencv.org/master/d2/d84/group__optflow.html)
