This files contains a collection of extra MuJoCo environments.

## HumanoidPendulum
The Humanoid Robot, but with objective of remaining standing up, instead of walking forward. (A Humanoid Version of "InvertedDoublePendulum")
```py
import gymnasium

gymnasium.make(
  "Humanoid-v5",
  forward_reward_weight=0,
  ctrl_cost_weight=0.2,
  contact_cost_weight=0,
  include_cinert_in_observation=False,
  include_cvel_in_observation=False,
  include_qfrc_actuator_in_observation=False,
  include_cfrc_ext_in_observation=False,
)
```

## CoupledHalfCheetah
2 HalfCheetas coupled together with a tendon.

Can be found at https://github.com/Farama-Foundation/Gymnasium-Robotics/blob/main/gymnasium_robotics/envs/multiagent_mujoco/coupled_half_cheetah.py


## Striker and Thrower 
https://github.com/RushivArora/Gym-Mujoco-Archive

## Unitree Go1
`xml_file` can be found at https://github.com/google-deepmind/mujoco_menagerie
```py
import gymnasium

env = gymnasium.make(
    'Ant-v5',
    xml_file='./mujoco_menagerie/unitree_go1/scene.xml',
    forward_reward_weight=1,
    ctrl_cost_weight=0.05,
    contact_cost_weight=5e-4,
    healthy_reward=1,
    main_body=1,
    healthy_z_range=(0.195, 0.75),
    include_cfrc_ext_in_observation=True,
    exclude_current_positions_from_observation=False,
    reset_noise_scale=0.1,
    frame_skip=25,
    max_episode_steps=1000,
)
```
 you can read more details at the tutorial: https://gymnasium.farama.org/main/tutorials/gymnasium_basics/load_quadruped_model/
