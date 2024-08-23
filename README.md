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
  

- Open new linux terminal and type this commands to linux terminal
  ```
  $ roscore
  # Open another new terminal and type this
  $ rosrun rosserial_python serial_node.py _port:=/dev/ttyACM0 _baud:=115200
  ```

- Go to "/Chair-TypeAsymmetricalTripedalRobot-main" directory
  ```
  $ cd /[SUBDIRECTORY]/Chair-TypeAsymmetricalTripedalRobot-main
  ```
