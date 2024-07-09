# TASK1 : Robot-walking-algorithm

## Table of Contents⚙️
- [Project Description](#project-description)
- [Technologies Used](#technologies-used)
- [Algorithm Explanation](#algorithm-explanation)
- [File Structure](#file-structure)

## Project Description📝


## Technologies Used 🔧
 - **Pseudocode**

## Algorithm Explanation

This algorithm assumes a simple robot with two legs, leg moves forward or backward during each step, each having three degrees of freedom: hip, knee, and ankle.
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
    MoveLeg("left", step_length, step_height, time )
    MoveLeg("right", -step_length, 0, time )
    MoveLeg("right", step_length, step_height, time )
    MoveLeg("left", -step_length, 0, time )
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




[def]: algorithm-explanation