
## HumanoidPendulum
The Humanoid Robot, but with objective of remaining standing up, instead of walking forward. (a Humanoid Version of "InvertedDoublePendulum")
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
