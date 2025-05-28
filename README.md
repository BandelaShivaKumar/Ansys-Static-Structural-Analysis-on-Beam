# Ansys-Static-Structural-Analysis-on-Beam
Static Structural Analysis on Beam- Stress,Strain,Total Deformation in Ansys(Project 2)
# 📐 Static Structural Analysis of a 3D Beam in ANSYS (Project 2)

(My Youtube Channel) Project Direct Youtube Link - https://youtu.be/h6KB-ocLbcM

This project demonstrates the static structural analysis of a 3D beam subjected to a point load (pressure from a monkey) using ANSYS 2025 R1. The objective is to determine the **equivalent (von-Mises) stress**, **total deformation**, and **strain distribution** across the beam.

## 🛠️ Software Used

- **ANSYS Mechanical**: 2025 R1
- **Workbench Environment**
- **OS**: Windows 11

---

## 📋 Problem Definition

Problem Image - https://github.com/BandelaShivaKumar/Ansys-Static-Structural-Analysis-on-Beam/blob/main/Problem%20Image/Screenshot%202025-05-19%20153141.png

Analyze a 3D beam under loading due to a monkey's weight sitting on a small region.

### 📏 Beam Dimensions (in meters):
| Parameter        | Value    |
|------------------|----------|
| Length           | 1.0 m    |
| Width (cross-section)  | 0.1 m    |
| Height (cross-section) | 0.1 m    |

### 🐒 Load Details:
- **Weight of monkey**: 30 kg
- **Pressure applied**: ~30,000 Pa
- **Load Area**: 0.01 m²
- **Force direction**: Vertically downward

---

## 🧱 Material Properties (Wood):

| Property           | Value         |
|--------------------|---------------|
| Young’s Modulus (E)| 8 × 10⁹ Pa    |
| Poisson’s Ratio (ν)| 0.3           |

---

## ⚙️ Boundary Conditions

| Condition          | Description                    |
|--------------------|--------------------------------|
| Fixed Support      | Right face of the beam         |
| Pressure Applied   | Left top surface (0.1 m length) where the monkey sits |

---

## 🧪 Meshing Details

| Setting             | Value             |
|---------------------|------------------|
| Element Type        | Hexahedral        |
| Mesh Relevance      | Medium-Fine       |
| Number of Elements  | ~90               |
| Size Control        | Automatic         |

---

## 📊 Results Summary

Results Images - Directional Deforamtion - https://github.com/BandelaShivaKumar/Ansys-Static-Structural-Analysis-on-Beam/blob/main/Images%20step%20by%20step%20process/Screenshot%202025-05-19%20201910.png

### 📌 Equivalent Stress (von-Mises):

| Metric     | Value         |
|------------|---------------|
| **Max**    | 1.7366 × 10⁶ Pa |
| **Min**    | 3484.2 Pa     |

### 📌 Total Deformation:
Total Deformation- https://github.com/BandelaShivaKumar/Ansys-Static-Structural-Analysis-on-Beam/blob/main/Images%20step%20by%20step%20process/Screenshot%202025-05-19%20202644.png
- Maximum observed at free end near the load application.
- Minimal at fixed support region.

### 📌 Strain Distribution:
 Maximum Principal Elastic Strain - https://github.com/BandelaShivaKumar/Ansys-Static-Structural-Analysis-on-Beam/blob/main/Images%20step%20by%20step%20process/Screenshot%202025-05-19%20202709.png
- Linear distribution observed along the length due to bending.
- Maximum strain at the top outermost fiber (in tension side).

---

## 📈 Visualization

Equivalent Stress - https://github.com/BandelaShivaKumar/Ansys-Static-Structural-Analysis-on-Beam/blob/main/Images%20step%20by%20step%20process/Screenshot%202025-05-19%20202653.png

> Tip: For better visual interpretation, enable contour legend, minimum/maximum probe markers, and vector arrows in the result section.

---

## 📂 Project Files Structure

```bash
Project2_Beam_Analysis/
├── geometry.agdb
├── beam_simulation.wbpj
├── Screenshot_2025-05-19_202653.png
├── Screenshot_2025-05-19_153141.png
└── README.md
📚 References
ANSYS 2020 R2 Tutorial – "Not Real Engineering"

ANSYS Learning Hub & Documentation

Mechanics of Materials by R.C. Hibbeler

✅ Conclusion
The ANSYS simulation successfully captures the stress concentration, deformation pattern, and boundary behavior of a 3D beam under a simplified real-world loading condition. This serves as a foundational problem for more complex FEA simulations.

📬 Contact
Author: Bandela Shiva Kumar
Mechanical Engineering Student- Btech
Business Email - BandelaLearns@gmail.com

Let me know if you'd like this in HTML or converted to a GitHub Pages site layout.
