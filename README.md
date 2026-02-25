# GIMloco: Generic Internal Model-Based Locomotion for Quadruped Robots

PyTorch implementation of GIMloco method which based on [HIMloco](https://github.com/InternRobotics/HIMLoco) and [rsl_rl]([https://github.com/leggedrobotics/rsl_rl]). If you use our code or data please cite the [paper].

Method is trained and tested on [IsaacGymEnvs](https://github.com/isaac-sim/IsaacGymEnvs).

Networks are trained using [PyTorch 1.2](https://github.com/pytorch/pytorch) and Python 3.7.

### Usage

The paper results can be reproduced by running:

* `cd legged_gym/legged_gym/scripts`
* `python train.py`

### Major work

There are two major difference with [HIMloco](https://github.com/InternRobotics/HIMLoco), the encoder of observation history become Generic Internal Model(GIM), and the Actor Net  input combine the GIM and one-step observation.

The hyper parameters of GIM include the decay rate, lenth of observation history, dimentions of internal model. All of these parameters effects the training and testing results.


### Bibtex

@inproceedings{yan2025GIMloco,
title={GIMloco: Generic Internal Model-Based Locomotion for Quadruped Robots},
author={Zhonghuai Yan, Quan Quan},
booktitle={2026 IEEE International Conference on Robotics and Automation (ICRA)},
year={2026}
}
