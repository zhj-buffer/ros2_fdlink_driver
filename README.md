# ros2_fdlink_driver

```
mkdir -p dev_ws/src && cd dev_ws/src && git clone https://github.com/zhj-buffer/ros2_fdlink_driver.git
cd ../ && colcon build 

source install/setup.bash
```



# Launch 
```
nvidia@nvidia-desktop:~/workspace/alan/fdlink_ahrs$ ros2 launch fdlink_ahrs ahrs_driver.launch.py                                                                    
[INFO] [launch]: All log files can be found below /home/nvidia/.ros/log/2021-12-31-16-46-34-830479-nvidia-desktop-3760 
[INFO] [launch]: Default logging verbosity is set to INFO 
[INFO] [ahrs_driver_node-1]: process started with pid [3763] 
[ahrs_driver_node-1] [INFO] [1640940445.044697606] [ahrs_bringup]: ahrsBringup::processLoop: start 
```

```
nvidia@nvidia-desktop:~/workspace/alan/fdlink_ahrs$ ros2 topic echo /mag_pose_2d 
x: 0.0 
y: 0.0
theta: 3.0803840297019294
---
x: 0.0 
y: 0.0
theta: 3.084585320100886
---
x: 0.0 
y: 0.0
theta: 3.0971622208842295
---
```

```
nvidia@nvidia-desktop:~/workspace/alan/fdlink_ahrs$ ros2 topic echo /imu 
header: 
  stamp:
    sec: 1640940867
    nanosec: 883843749
  frame_id: gyro_link
orientation:
  x: 0.0006944536170621562
  y: 0.004044804318867822
  z: -0.9268403988083694
  w: -0.3754333082416843
orientation_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
angular_velocity:
  x: 8.523184806108475e-05
  y: 0.0013440082548186183
  z: -0.0065114181488752365
angular_velocity_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
linear_acceleration:
  x: -0.011358600109815598
  y: 0.07851383090019226
  z: -9.857669830322266
linear_acceleration_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
---
```

```
---
header:
  stamp:
    sec: 1641605909
    nanosec: 574721115
  frame_id: imu_link
orientation:
  x: 0.0038386048691728338
  y: 0.0008561068979948812
  z: 0.04856155691346975
  w: -0.9988125474857716
orientation_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
angular_velocity:
  x: 0.0004518600180745125
  y: 0.00013582047540694475
  z: 0.00022458471357822418
angular_velocity_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
linear_acceleration:
  x: -0.019728094339370728
  y: 0.0755247175693512
  z: -9.841728210449219
linear_acceleration_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
---
header:
  stamp:
    sec: 1641605909
    nanosec: 584707868
  frame_id: imu_link
orientation:
  x: 0.0038380444466005205
  y: 0.0008535819626863071
  z: 0.04856491339710582
  w: -0.9988123090601326
orientation_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
angular_velocity:
  x: 7.999595254659653e-06
  y: -0.00021926744375377893
  z: -0.0005743633955717087
angular_velocity_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
linear_acceleration:
  x: -0.034075796604156494
  y: 0.06356830149888992
  z: -9.848703384399414
linear_acceleration_covariance: [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]
---
```
