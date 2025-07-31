# CMC_ElbowFlexion_Dynamics
## 🔍 Overview

This repository contains a focused subset of the **Elbow_Loading_Simulation** project, specifically highlighting the custom modifications applied to the control and motion files of the `arm26` musculoskeletal model using **OpenSim**.

These modifications were performed as part of a task aiming to explore the effects of different control strategies and motion inputs on muscle coordination, joint kinematics, and simulation outcomes.

---

## 📁 Repository Structure


Elbow_Loading_Simulation/
│
├── ModifiedControls/
│ ├── arm26_ControlConstraints1.xml
│ ├── arm26_ComputedMuscleControl_Tasks1.xml
│ └── arm26_SpecifiedShoulder.mot
│
└── report.pdf

نسخ
تحرير

---

## 🛠️ What We Changed

### 1. `arm26_ControlConstraints1.xml`
- Modified the control constraints to limit muscle activations for specific groups (e.g., long head of biceps).
- Purpose: To observe how restricting certain muscle groups affects compensation by others.

### 2. `arm26_ComputedMuscleControl_Tasks1.xml`
- Changed task priorities and tracking weights in the Computed Muscle Control (CMC) tool.
- Purpose: To investigate the impact of task weighting on motion accuracy and muscle force generation.

### 3. `arm26_SpecifiedShoulder.mot`
- Edited motion file to specify a fixed shoulder angle throughout the motion.
- Purpose: To assess the biomechanical consequences of locking shoulder movement.

---

## 📊 Results

Results from each modification are saved under the corresponding folder in `Results/`:

- **ControlConstraints1/**: Effects of limiting biceps long head.
- **Tasks1/**: Comparison between default and custom task priorities.
- **SpecifiedShoulder/**: Resulting kinematics with frozen shoulder movement.

Each folder contains joint angles, muscle activations, and other simulation outputs exported from OpenSim.

---

## 📄 Report

For detailed analysis, figures, and interpretation of the results:
- See [`report.pdf`](./report.pdf)

---

## 📎 Requirements

This work was performed using:
- OpenSim version: `4.5`
- Model used: `Arm26.osim` (standard OpenSim model)

---

## 👥 Contributors

This project was collaboratively developed by a dedicated team of students from the System and Biomedical Engineering Department, Cairo University:
_**Amatalrahman Sayed**
_**Alaa Essam**
_**Saja Sadek**
_**Ziad Osama**
_**Hassan Badawy**


---

## 📌 Notes

This repository **does not** include the full simulation setup or OpenSim default files. It only includes:
- Modified control/motion files.
- Results corresponding to those modifications.
- A summary report.

For full OpenSim installation and model structure, refer to the [official OpenSim website](https://simtk.org/projects/opensim).


