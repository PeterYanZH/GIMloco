# GIMloco: Generic Internal Model-Based Locomotion for Quadruped Robots

PyTorch implementation of the GIMloco method, which is based on [HIMloco](https://github.com/InternRobotics/HIMLoco) and [rsl_rl](https://github.com/leggedrobotics/rsl_rl). If you use our code or data, please cite the [paper].

Method is trained and tested on [IsaacGymEnvs](https://github.com/isaac-sim/IsaacGymEnvs).

Networks are trained using [PyTorch](https://github.com/pytorch/pytorch) and Python 3.8.

### Usage

The paper results can be reproduced by running:

* `cd legged_gym/legged_gym/scripts`
* `python train.py`

### Major work

There are two major differences with [HIMloco](https://github.com/InternRobotics/HIMLoco), the encoder of observation history become Generic Internal Model(GIM), and the Actor Net  input combines the GIM and one-step observation.

The hyperparameters of GIM include the decay rate, length of observation history, and dimensions of the internal model. All of these parameters affect the training and testing results.


### Bibtex

```
@inproceedings{yan2025GIMloco,
title={GIMloco: Generic Internal Model-Based Locomotion for Quadruped Robots},
author={Zhonghuai Yan, Quan Quan},
booktitle={2026 IEEE International Conference on Robotics and Automation (ICRA)},
year={2026}
}
```
