# Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time
This repository contains the dataset of the Sensors 2022 paper `Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time`.

---
## File formats

* **real**
    This data contains the Inertial Measurements Units (IMUs) data from 6 [Xsens DOT](https://www.xsens.com/xsens-dot) and full-body joints data from OptiTrack.
* **synth**
    This data contains the synthesized IMU data from 3d human motion.

Each npz file store a dictionary as:
- x: a numpy array of shape (N, 430), head height (1) + sensor# (6) * feature# (quaternions (4) + acceleration (3))
- y: a numpy array of shape (N, 146), joint_pos + joint_ros
  - joint_pos: a numpy array of shape (N, 62)
  - joint_ros: a numpy array of shape (N, 84)

## About Data
```
FusionPoser/
    -Dataset/
        -real/
            -motion_0625173852_x.npz
            -motion_0625173852_y.npz
            -...
        -synth/
            -07_01_x.npz
            -07_01_y.npz
    -LICENSE
    -README.md
```
## License
This project is licensed under the MIT License.

## Citation
This is the official dataset of the paper "Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time"

If you find the project helpful, please consider citing us:
```
@Article{Kim_Sensors_2022_FusionPoser,
AUTHOR = {Kim, Meejin and Lee, Sukwon},
TITLE = {Fusion Poser: 3D Human Pose Estimation Using Sparse IMUs and Head Trackers in Real Time},
JOURNAL = {Sensors},
VOLUME = {22},
YEAR = {2022},
NUMBER = {13},
ARTICLE-NUMBER = {4846},
URL = {https://www.mdpi.com/1424-8220/22/13/4846},
PubMedID = {35808342},
ISSN = {1424-8220},
DOI = {10.3390/s22134846}
}
```
