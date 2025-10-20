## 🤖 Sandman GUI (PyQt + ROS + Joystick)

> ⚠️ **Note:**  
> This repository is a **public copy** of a private project originally developed under the **AURobotics organization** — a technical subteam for my university.  
> The code was recreated and published here for **academic and demonstration purposes** only.

---

## 🧠 Overview

This project provides an **interactive GUI simulator** for a ROS-based robot performing **mine detection** and movement control.  
It combines **PyQt5** for the interface, **Matplotlib** for visualizing the minefield, **pygame** for joystick input, and **ROS** for real-time communication.

The application visualizes a 19×19 minefield grid and allows real-time robot movement and mine detection updates through ROS topics.  
Users can also control the robot using a **PlayStation controller**, and monitor buried and surface mines via interactive tables.

---

## ⚙️ Features

- 🧭 **Real-Time Robot Tracking** – Displays robot position updates from the `/robot_location` topic.  
- 💣 **Mine Visualization** – Marks buried and surface mines dynamically on the grid when messages arrive on `/mine_location`.  
- 🕹️ **Joystick Support** – Reads PlayStation or generic controller input using `pygame` and publishes data to `/controller_states`.  
- 📊 **Mine Tables** – Displays coordinates of buried and surface mines separately.  
- 🖼️ **Customizable Map** – Clean, labeled grid layout rendered using Matplotlib.  
- 🔄 **ROS Integration** – Publishes and subscribes to topics for real-time data exchange.
