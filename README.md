# 🤖 Self-Driving Robot with Single and Stereo Camera Vision 🚗

## 💡 Overview

This project features a self-driving robot designed to navigate towards a sequence of markers, using:

- Stereo Vision: Two cameras calculate depth and angle through disparity measurements.
- Single-Camera Vision: Estimates distance and angle based on marker size, using reference measurements.

The robot adjusts its movement dynamically based on the marker’s color and position:

🟢Green: Full speed

🟡Yellow: Slow speed

🔴Red: Stop

## ⚙️ Features

### Dual Vision Modes:

- Precise depth and angle estimation with stereo vision.
- Simplified single-camera setup with intelligent fallback strategies.

### Color-Based Speed Control:

- Green: Full speed
- Yellow: Slow speed
- Red: Stop

### Dynamic Navigation:

- Adjusts direction and speed based on marker position.
- Rotates to locate markers outside the frame.

### Error Handling:

- Ensures reliable distance estimation with contour checks.
- Manages partial marker visibility and limited fields of view.

## 👩‍💻 Technologies Used

### Hardware:

  🛠️LEGO EV3 brick

  🛠️Dual or single camera setup

### Software:

  💻Python (OpenCV for vision, EV3Dev2 for robot control)
  
  💻IP Webcam for wireless video streaming

### Networking:

  🛜TCP server-client architecture for robot-laptop communication

## 🔍 How It Works

### 👀 Stereo Vision Mode

- Disparity Calculation: Depth is determined by the difference in marker positions between camera frames.
- Angle Calculation: The horizontal offset from the camera center determines the angle.
- Robot Movement: Adjusts wheel angle and speed to navigate to the marker.

### 👁️ Single-Camera Vision Mode

 - **Distance Scaling:** Distance (cm) = (Reference Distance × Reference Marker Radius) ÷ Next Marker Radius
 - **Angle Calculation:** Based on the marker's horizontal displacement.
 - **Fallback Strategies:** Rotates to find markers outside the frame.

## 🏗️ Design

### Steering Mechanism
Utilizes 5 gears for precise control:
- A central gear turns two outer gears via smaller intermediary gears.
- This ensures equal steering angles for both wheels, maintaining alignment during turns.

## 🤓 Extra Info

- Made for CMPUT 312 Final Project
- Team Members: Mekha George, Maher Maher

## Images of Car
<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/7a5ed243-8401-4e5f-aa14-749a0927de6d" width="300"></td>
    <td><img src="https://github.com/user-attachments/assets/89dce1ad-2f94-4cbd-bab6-cd6c29e9effc" width="300"></td>
    <td><img src="https://github.com/user-attachments/assets/f203c066-472a-45dd-9825-24bc02d6efa4" width="300"></td>
  </tr>
</table>


