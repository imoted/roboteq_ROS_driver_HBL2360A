# roboteq_diff_driver

ROS driver for the Roboteq HBL2360A of motor controllers in a differential-drive configuration.
I guess it can also aply to the other Blushless Roboteq driver.
But it needs to find the proper PID parameter of each motors.

Subscribes to cmd_vel, publishes to odom, and broadcasts odom tf.

Also publishes sensor data to some ancillary topics including roboteq/voltage, roboteq/current, roboteq/energy, and roboteq/temperature.

Does not require any MicroBasic script to operate.

## Usage

Clone to src directory of catkin workspace, then `catkin build`.

Requires ROS serial package. If not already installed:
```
sudo apt-get install ros-<dist>-serial
```

Sample launch files in roboteq_diff_driver/launch.

## License

This project is licensed under the BSD License.

