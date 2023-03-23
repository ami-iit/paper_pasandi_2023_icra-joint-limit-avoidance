## Torque Control of the humanoid robot iCub

The Simulink model for simulating the torque control with joints position and velocity limits avoidance for controlling the right leg of humnaoid robot iCub in Gazebo while it is on the poll.

<div align="center">
<img src="https://user-images.githubusercontent.com/34647611/227213946-7d533217-2b4a-498b-a186-fcbcbef69d5d.png" width="300">
</div>

### How to Run

1. Set the environmental variable YARP_ROBOT_NAME by adding the following line in the .bashrc:
```
export YARP_ROBOT_NAME=iCubGazeboV2_5
```
2. Verify that Gazebo and the robot model for simulations are available and installed. You can check if the controller is targeting the correct robot model by typing on a terminal:
```
yarp resource --find model.urdf
```
then, check that the path and the model name are correct.
3. Launch the `yarpserver` by typing in a terminal
```
yarpserver --write
```
4. Launch gazebo. It is in general required to use the synchronization between the controller and the simulator to avoid real-time factor related problems. Therefore launch gazebo by typing in a terminal:
```
gazebo -slibgazebo_yarp_clock.so
```
5. Insert the robot model `iCubGazeboV2_5_fixed` in Gazebo.
6. Open MATLAB
7. Open [main.mlx](main.mlx)
8. Set the system configuration parameters, including
  - joints position and velocity limits,
  - desired joints trajectory,
  - coefficients of controller,
9. Run the script
