# TASK1 : Robot-walking-algorithm

## Table of Contents⚙️
- [Project Description](#project-description)
- [Technologies Used](#technologies-used)
- [Algorithm Explanation](#algorithm-explanation)
- [File Structure](#file-structure)

## Project Description📝
This algorithm is designed for a simple robot with servo motors controlling two legs. Each leg has three degrees of freedom: the hip, knee, and ankle joints. The robot's walking motion is achieved by moving the legs forward and backward during each step.

The process begins by initializing the servo motors and setting the initial position of the robot. Walking parameters such as step length, step height, and time are obtained using the Get function. The main walking cycle involves alternating movements of the left and right legs, with each leg either lifting and moving forward or moving backward while staying on the ground.

The MoveLeg function calculates the necessary angles for the hip, knee, and ankle joints based on the given step parameters. By continuously repeating the walking cycle, the robot achieves a coordinated and stable walking motion. This approach ensures that the robot maintains balance while simulating a natural gait.

## Technologies Used 🔧
 - **Pseudocode**

## Algorithm Explanation

This algorithm assumes a simple robot with servo motors and two legs, leg moves forward or backward during each step, each having three degrees of freedom: hip, knee, and ankle.
```
 // Initialize servo motors
InitializeServos()

// Set initial position
SetInitialPosition()

// Define walking parameters using Get function
step_length = Get("step length")
step_height = Get("step height")
time = Get("time")

// Walking cycle function
Function Walking()
    MoveLeg("left", step_length, step_height, time ) // left leg moves forward
    MoveLeg("right", -step_length, 0, time ) // right leg moves backward and zero because leg is being moved backward without lifting it
    MoveLeg("right", step_length, step_height, time ) // right leg moves forward
    MoveLeg("left", -step_length, 0, time ) // left leg moves backward
End Function

// Function to move a leg
Function MoveLeg(leg, length, height, time)
    SetHipAngle(leg, length)  // Calculate hip angle based on step length
    SetKneeAngle(leg, height )  // Calculate knee angle based on step height
    SetAnkleAngle(leg, height ) // Calculate ankle angle based on step height
End Function

// Function to get parameters (assuming input from user or sensors)
Function Get(parameter)
    Return ReadInput(parameter)
End Function
```

## File Structure 🏗️

```
Robot-walking-algorithm/
│
├── README.md
```

- `README.md`: This file, containing information about the project.

made with love by "she codes team "🤍😄
raghad Alshammari - sadeem alresaini - razan alothaim.
