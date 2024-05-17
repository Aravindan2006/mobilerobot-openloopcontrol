# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

### Step1:
 Initiate the MobileRobot.

### Step2:
 Connect your PC with the MobileRobot.

### Step3:
 Open Python program.

### Step4:
 Program the movements of the robot using python code.

### Step5:
 Execute the python program.



## Program

#NAME : ARAVINDAN D
#REGISTER NO: 212223240012

```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=0, y=3.05, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=200,g=255,b=205,effect="on")

    ep_chassis.move(x=1.16, y=0, z=15, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=255,b=255,effect="on")
    
    ep_chassis.move(x=0, y=0, z=75, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=153,b=102,effect="on")

    ep_chassis.move(x=1.25, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=204,b=255,effect="on")

    ep_chassis.move(x=0, y=0, z=-40, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=1.68, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=192,g=192,b=192,effect="on")

    ep_chassis.move(x=0, y=0, z=43, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=135,g=151,b=0,effect="on")


    ep_chassis.move(x=1.3, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=51,b=51,effect="on")

   

    ep_chassis.move(x=0, y=-2, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=255,b=255,effect="on")

    ep_chassis.move(x=0, y=0, z=-90, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=255,effect="on")

    ep_chassis.move(x=-0.2, y=.7, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=102,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")





    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./img/robomaster.png)



![movementimg](https://github.com/Aravindan2006/mobilerobot-openloopcontrol/assets/151760062/b47d3a8e-b069-4646-a69d-34ff179d8aa6)




## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

https://youtu.be/wtgheN4woao?feature=shared


## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.




```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
