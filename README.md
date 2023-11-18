# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)
```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/plotswag/Movement-of-Robot-Joints/assets/145822344/ecdc51be-a5d5-4412-84b3-6a15d4ffb943)


### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/plotswag/Movement-of-Robot-Joints/assets/145822344/4617f3f3-1217-489e-85b5-4244b71d2828)

### 3. Movement of Joint1
![image](https://github.com/plotswag/Movement-of-Robot-Joints/assets/145822344/4f14df6a-f3a5-4bbd-bac6-a6562862e20b)


### 3. Movement of Joint2
![image](https://github.com/plotswag/Movement-of-Robot-Joints/assets/145822344/18712ba7-2cc7-477c-b483-6692254acc67)


### 3. Movement of Joint3
![image](https://github.com/plotswag/Movement-of-Robot-Joints/assets/145822344/9c955a59-b580-4f93-866b-97c936b88c43)

## Result 
Thus the different robots joints are moved with the help of python list.


