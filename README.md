# 3DLine-SLAM
# 3DLine-SLAM
# 3DLine-SLAM
基于ORB-SLAM的单目视觉实时半稠密地图重建
构建更详细的地图和定位更精准的相机姿态一直都是同时定位与制图(SLAM)技术的目标，但是以上目标同实时性要求、较低的计算花费和低廉的硬件条件是相矛盾的。本文提出一种基于单目ORB-SLAM方法上匹配关键帧中提取到的直线特征重构半稠密三维场景的方法。首先由ORB-SLAM实时提供一组关键帧及其对应的相机位姿以及一系列地图点。然后使用新提出的关键帧再剔除算法减少冗余帧数目。再使用改进的直线段提取方法提取各帧中的直线段。最后使用纯几何约束的方法匹配以上检测到的直线段来生成场景的三维模型。通过深入地分析与彻底的实验评估，结果表明新方法能持续稳定的运行，整个系统具有较强的鲁棒性，且能在低计算花费条件下快速的在线进行三维重构。
A Monocular-vision Semi-dense 3D Reconstruction Based on ORB-SLAM
Abstract：Producing high-quality 3D maps and calculating more accurate camera pose have always been the goal of Simultaneous Localization and Mapping (SLAM) technology. The requirements of SLAM such as real-time, low computational cost, and low hardware cost are contradictory to the above objectives. For the issues listed above, we propose a novel semi-dense reconstruction method based on the monocular ORB-SLAM by matching the line segment features extracted from keyframes. Specifically, our method builds upon ORB-SLAM, which first outputs a set of keyframes and their corresponding camera poses and a series of map points in real-time. To reduce redundant keyframes, we develop a keyframe culling algorithm (KRC). Then an improved line segment extraction algorithm is adopted to extract line segments in each keyframe. Finally, we use purely geometric constraints to generates accurate 3D scene model by matching 2D line segments from different keyframes. We thoroughly evaluate and analyse our approach. Experimental results show that our method runs steadily and reliably. This whole method has strong robustness and it also can quickly generate an accurate 3D scene online.
