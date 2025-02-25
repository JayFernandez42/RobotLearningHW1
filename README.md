# CS 4756/5756: Robot Learning - Assignment 2
This repository contains the implementation of imitation learning techniques to train a Fetch robot on the Reach task using expert demonstrations. 
The assignment was completed in Google Colab using Gymnasium Robotics' Mujoco Environments.

## Implemented Techniques

#### Behavior Cloning (BC): 
- Trains an agent using supervised learning on a dataset of expert demonstrations.

- Optimized via cross-entropy (discrete actions) or mean-squared error (continuous control).

- Implemented a training loop that updates the policy and monitors validation loss to check for overfitting.

#### Dataset Aggregation (DAgger): 

- Improves upon BC by allowing the agent to query the expert dynamically.

- Starts with the BC-trained model, collects new data by interacting with the environment, and refines the policy.

- Helps the agent recover from suboptimal states, leading to improved performance over BC alone.

## Implementation Notes

 - Colab's T4 runtime is recommended
   
 - Training should take ~1 minute for BC and ~2 minutes for DAgger.

