# Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time
This repository contains the dataset of the paper `Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time`.

---
## File formats

* **data-0625**
This data contains the Inertial Measurements Units (IMUs) data from 6 [Xsens DOT](https://www.xsens.com/xsens-dot) and full-body joints data from OptiTrack.
* **data-**

Each pickle file storea a dictionary as:
- imus: a numpy array of shape (N, 6, 7*) * quaternions(4) + acceleration(3)
- joint_pos: a numpy array of shape (N, ) 
- joint_ros: a numpy array of shape (N, )

## About Data
```
FusionPoser/
    -data-0625/
        -data_0625173852.pkl
        -...
    -data-/
        -data_.pkl
        -...
    -LICENSE
    -README.md

```
## License
This project is licensed under the MIT License.

## Citation
This is the official dataset of the paper "Fusion Poser: 3D Human Pose Estimation using Sparse IMUs and Head Tracker in real-time"

If you find the project helpful, please consider citing us:
