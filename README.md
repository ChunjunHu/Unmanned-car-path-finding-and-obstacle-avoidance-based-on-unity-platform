# Unmanned-car-path-finding-and-obstacle-avoidance-based-on-unity-platform
Unity3D + A* + DeepLearning(LanNet) + DWA + PID + Reinforcement Learning -> UnmannedCar

1. Our project currently realizes road recognition, path planning and vehicle obstacle avoidance;

2. Lane line recognition uses LaneNet neural network structure to sample the image, and uses monocular distance measurement to realize instance segmentation and binarization segmentation. The two sets of data obtained are processed by perspective transformation matrix, and finally the loss function is backpropagated to achieve Dynamically recognize lane lines and divide different lane labels;

3. Path planning uses A* global planning algorithm to select the optimal path;

4. The obstacle avoidance function combines the DWA algorithm with reinforcement learning to assign different weights to the two methods, and combines the return value with the accelerator brake steering booster to achieve vehicle obstacle avoidance. The PID control algorithm is used in simulating vehicle speed and steering stability, which solves the problem of sudden acceleration, deceleration, sharp cornering and jitter.
