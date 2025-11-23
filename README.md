# 🌿 Design of a Plant Wearable Device for Assessing Microclimate’s Impact on Plant Growth

<p align="center">
  <img src="images/Picture1.PNG" alt="AgriBot CAD Model" width="600"/>
</p>

## 🚀 Overview

AgriBot is a four-wheel drive and four-wheel steerable robotic platform designed for precision agriculture tasks, including **targeted fertilization** and **real-time plant inspection**, specifically tailored for cabbage farming over moderately rugged terrain. The robot aims to enhance agricultural productivity and reduce labor involvement using **autonomous mobility**, **suspension system**, **image-based disease detection**, and **ROS-based control integration**.

---

## 🌱 Application Domain

The robot addresses key challenges in smart agriculture:

- **Precision nutrient application** to avoid overuse of fertilizers.
- **Real-time monitoring** of plant health using computer vision.
- Operation in **rugged and uneven terrains** typical to open-field farming.
- **Remote data acquisition** and daily reports for farmers.

---

## 🧠 Key Modules and Analysis

### 🛠 Mechanical Design

- **Chassis**: X-frame-based for enhanced stability and modularity.
- **Liquid Tank**: Baffled design with HDPE material to minimize CG shifts.
- **Suspension**: Parallelogram mechanism to ensure camera stability and traction in rough terrains.

<p align="center">
  <img src="images/Picture2.png" alt="Chassis and Suspension" width="600"/>
</p>

---

### 📐 Structural and Dynamic Analysis

- **Material selection** using ANSYS FEA simulations comparing multiple combinations.
- **Topology optimization** for wheel bracket to reduce weight.
- **Suspension damping analysis** for stability under dynamic loads.
  
<p align="center">
  <img src="images/Picture 3.PNG" alt="ANSYS Results" width="500"/>
</p>

---

### 🔧 Kinematic & Control System

- **Four-wheel drive & steering** kinematic model developed in MATLAB.
- **PID-based path tracking** controller implemented to follow desired trajectories.
- **Dynamic torque analysis** using MSC ADAMS.

---

### 🤖 Embedded & ROS Integration

- **Drive and steering control** via Arduino microcontroller with timer interrupts.
- **ROS integration** for sensor communication and high-level control.
- Simulated in **Gazebo** and visualized via **RViz**.

---

### 💡 Vision System

- Used **YOLO** for real-time **leaf disease detection**.
- Built dataset with multiple diseased leaf images due to lack of cabbage-specific datasets.
- Trigger-based control: stops robot and activates pump upon detection.


---

## 🧪 Prototyping & Results

- Successfully integrated low-level Arduino code with high-level ROS nodes.
- Built a prototype for field testing, including a basic Ackermann steering system.
- Developed a **fertilizer spray system** responsive to vision-based commands.

---

## 📦 Tools & Technologies

- `SOLIDWORKS` for 3D modeling
- `MATLAB` for kinematic modeling
- `ANSYS` & `ADAMS` for structural/dynamic simulations
- `Arduino` for low level control
- `ROS (Noetic)` on `Ubuntu 20.04` for system integration
- `YOLO` for real-time object detection

---
