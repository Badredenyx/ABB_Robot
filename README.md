

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/Badredenyx/ABB_Robot/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

# ABB_Robot 🦾

Welcome to the ABB_Robot project! This repository contains a RobotStudio Pack&Go file and a simulation video demonstrating a palletizing, sorting, and pick & place example using an ABB industrial robot. Whether you’re learning RobotStudio or building industrial automation solutions, this tutorial-style project will help you get started with Smart Components, RAPID programming, digital I/O, and safety features.

## 🔍 Project Overview

- **Robot Model:** IRB 1660ID
- **Task:** Sort and palletize two box types using a suction cup vacuum gripper
- **Objects:**  
  - 3 small orange boxes (20×20×10 cm)  
  - 3 large green boxes (20×20×20 cm)  
- **Goal:** Stack each box type on its designated pallet side
- **Standards:** Implements ISO 10218:2011 safety elements (QuickStop, world zones)

## 📂 Repository Structure

```

Badredenyx/ABB\_Robot
├── ABB\_Robot\_Project.rspag          # RobotStudio Pack\&Go archive
└── Simulation Video.mp4             # Demo simulation video

````

---

## ⚙️ Installation

1. **Download the repository**
   ```bash
   git clone https://github.com/Badredenyx/ABB_Robot.git
   cd ABB_Robot


2. **Open in ABB RobotStudio**

   * Launch RobotStudio
   * File → Open → select `ABB_Robot_Project.rspag`
   * Follow the Unpack & Work wizard:

     1. Select target folder
     2. Choose RobotWare version 6.08.01.00 (IRB 1660ID)
     3. Finish unpacking and start simulation

> **Note:** Requires RobotStudio **6.08.01** and RobotWare **6.08.01.00** (IRB 1660ID).

---

## ▶️ Usage

1. Load the project into RobotStudio as above.
2. Switch to **Simulation** mode.
3. Press **Play** to run the palletizing sequence.
4. Observe the robot picking, sorting, and stacking the boxes using the suction gripper.

### 📹 Demo Video

<video src="Simulation Video.mp4" controls width="640">
Your browser does not support HTML5 video.
</video>

---

## 🔧 Configuration

* **Suction Cup Offset:** Adjust TCP offsets in the **Tool Data** tab.
* **Conveyor Speed:** Modify belt speed parameters in the **Conveyor** Smart Component properties.
* **Digital I/O:** Map your virtual I/O signals under Controller → I/O Configuration.

---

## 🛠️ Key Features & Tools

* **Smart Components**: Gripper and conveyor modeling
* **Work Objects & Offsets**: Precise pick & place trajectories
* **RAPID Code**: Custom box-handling logic and stacking
* **Digital Signals**: I/O-based suction control and sensors

---

## 📚 Tutorial Breakdown

1. **Suction Cup with Smart Components**

   * Import `.SAT` CAD model for gripper
   * Configure attach/detach via digital input

2. **Conveyor Setup**

   * Build belt with physics properties
   * Add photoelectric sensors and automations

3. **Pick & Place Logic**

   * Define Work Objects for pallets and conveyor

4. **Safety Integration**

   * Add QuickStop and world zone monitoring

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m "Add awesome feature"`
4. Push to branch: `git push origin feature/YourFeature`
5. Open a Pull Request

Please adhere to the existing coding style and conventions.

---

## 📝 License

Distributed under the MIT License. See [LICENSE](./LICENSE) for details.

