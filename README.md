# Structure Information is the Key: Self-Attention RoI Feature Extractor in 3D Object Detection

**abstract**:Unlike 2D object detection where all RoI features come from grid pixels, the RoI feature extraction of 3D point cloud object detection is more diverse. In this paper, we first compare and analyze the differences in structure and performance between the two state-of-the-art models PV-RCNN and Voxel-RCNN. Then, we find that the performance gap between the two does not come from point information, but structural information. Although the location information of the voxel features is fuzzier than the point features, the voxel features contain more structural information because they do quantization instead of downsampling to point cloud so that they can contain basically the complete information of the whole point cloud. The stronger structural information in voxel features makes the detector have higher performance in our experiments even if the voxel features don't have accurate location information. Then, we propose that structural information is the key to 3D object detection. Based on the above conclusion, we propose a Self-Attention RoI Feature Extractor (SARFE) to enhance structural information of the feature extracted from 3D proposals. SARFE is a plug-and-play module that can be easily used on existing 3D detectors. Our SARFE is evaluated on both KITTI dataset and Waymo Open dataset. With the newly introduced SARFE, we improve the performance of the state-of-the-art 3D detectors by a large margin in \textit{cyclist} on KITTI dataset and it can still maintain the real-time performance of the original detectors. 

+ The source code will be published after the paper has been accepted to a conference.

[Full paper](https://github.com/Poley97)

## AP on KITTI Dataset

[Submission link](http://www.cvlibs.net/datasets/kitti/eval_object_detail.php?&result=c68ef62ce6e1b03735673eb996b72c0fd9cbe159)
## AP on Waymo Open Dataset

[Submission link](https://waymo.com/open/challenges/entry/?challenge=DETECTION_3D&emailId=619cf721-2991&timestamp=1634972524047035)
## License
This code is released under the Apache 2.0 license.

## Acknowledge
Our code are mainly based on [OpenPCDet](https://github.com/open-mmlab/OpenPCDet), thanks for their contributions!