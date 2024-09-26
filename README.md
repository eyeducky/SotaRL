# ♡🤍♡🤍♡🤍♡🤍♡🤍I love Mr.Cha-Hyeongjun ♡🤍♡🤍♡🤍♡🤍♡🤍

## Environment
- Ubuntu 20.04 (64bit)
- ROS-Noetic 1.16.0
- Arduino IDE 2.3.2

## Usage
- Run ArduinoIDE and upload embedded code to Arduino
  ```
  $ ./arduino-ide_2.3.2_Linux_64bit.AppImage
  ```

### Set ROS serial environments

- Open Linux Terminal and type this commands to linux terminal
  ```
  $ roscore
  ```


- Go to "/Chair-TypeAsymmetricalTripedalRobot-main/launch" directory and load ROS parameters
  ```
  # Open new Linux terminal
  $ cd /[SUBDIRECTORY]/Chair-TypeAsymmetricalTripedalRobot-main/launch
  $ rosparam load param.yaml
  # If you get error about failed load parameter, delete paramload() in Arduino IDE code and except this
  ```
  
- Open another New Terminal and type this
  ```
  $ rosrun rosserial_python serial_node.py _port:=/dev/ttyACM0 _baud:=115200
  # You can see about serial data by typing '$ rostopic echo /sensor/[NAME]'
  ```

### Run model

- Open Linux Terminal
  ```
  $ cd /[SUBDIRECTORY]/Chair-TypeAsymmetricalTripedalRobot-main/src
  ./rl_stand.py
  ```
