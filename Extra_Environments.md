
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
