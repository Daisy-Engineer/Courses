# 🌊 GE3850: Geohydrology Syllabus - Spring 2026

---

## 📅 Course Information

* **Course Title:** Geohydrology, GE3850 
* **Semester:** Spring 2026 
* **Schedule:** Tuesday (1 hr lecture + 1 hr computer lab) & Thursday (1 hr lecture) 
* **Credits:** 3 
* **Instructor:** Daisy Ning, yning1@mtu.edu, Dow 405 
* **Textbook:** *Applied Hydrogeology*, 5th Edition, C. W. Fetter, David Kreamer 

---

## 📝 Course Description

This course introduces the physical and chemical principles governing groundwater flow and occurrence. It emphasizes the quantitative analysis of subsurface flow systems. Students will learn how to apply Darcy’s law, interpret aquifer properties, analyze groundwater flow using analytical and numerical methods, and understand groundwater contamination and management.

---

## 🎯 Course Objectives

By the end of the course, students will be able to: 

* Explain the occurrence, movement, and distribution of groundwater.
* Apply Darcy’s Law to different hydrogeologic conditions.
* Characterize aquifer properties using field and analytical data.
* Analyze steady and unsteady flow through analytical and numerical solutions.
* Construct and interpret groundwater flow models using MODFLOW.
* Understand contaminant transport and basic remediation concepts.
* Relate hydrogeologic principles to groundwater resource management.

---

## 💻 Software and Tools

* **Python:** For analytical and plotting tasks.
* **GMS (Groundwater Modeling System) - MODFLOW**

---

## 📊 Assessment

| Component | Weight |
| :--- | :--- |
| Homework | 20% |
| Labs | 20% |
| Midterm Exam | 20% |
| Final Project / Presentation | 15% |
| Final Exam | 25% |

* **Homework Policy:** Your **two lowest homework scores** will be **dropped** from the final grade calculation. This helps provide flexibility for occasional difficulties or schedule conflicts.

### Grading and Regrade Requests
Homework, lab assignments, and exams will be **graded by the course Teaching Assistant (TA)**.

- **Regrade requests** should be submitted **directly to the TA** within **7 calendar days** of the assignment being returned.
- Extensions due to emergencies or health issues should be requested **before the due date** when possible.

---

## 📆 Weekly Schedule (Spring 2026)

**(Tues = Lecture + Lab, Thurs = Lecture)** 

| Week | Date (Week of)    | Tue Lecture                                 | Tue Lab (Python + Modflow)                                                                                     | Thu Lecture                                                | Fetter Chapters | HW                     | Notes                                                        |
|------|----------|-----------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|-----------------|-------------------------|--------------------------------------------------------------|
| 1    | 1/6/26   | **Ch 1: Introduction**  | Python + Hydro Data Analytics: Jupyter intro, units, load precipitation–streamflow data, compute annual water balance | **Ch 2.5–2.8: Water Balance, Precipitation, ET, Infiltration, Recharge**   | Ch 1; 2.1–2.4   | Ch 1 (1,3,5,13); Ch 2 (1) |                                                              |
| 2    | 1/13/26  | **Hydrographs (Ch 2.5–2.8)**                 | Hydrograph Analysis: Baseflow separation, smoothing, runoff volume, hydrograph plotting in Python                             | **Runoff, Recharge, Manning (Ch 2.9–2.14)**                 | 2.9–2.14        | Ch 2 (9, 12, 13, 17)      |                                                              |
| 3    | 1/20/26  | **Porosity & Void Ratio (Ch 3.1–3.2)**        | Porosity & Grain Size: Compute D10–D60, grain-size curves using numpy, porosity estimation                                     | **Specific Yield & Retention, Hydraulic Conductivity (Ch 3.3-3.4)**               | 3.1–3.33        | no HW       |                                                              |
| 4    | 1/27/26  | **Hydraulic Conductivity Measurement, Water Table (Ch 3.5-3.6)**           | K Measurement: Compute K from constant-head & falling-head tests; curve fitting using scipy                                    | **Aquifer Characteristics, Potentiometric Surface (Ch 3.7, 3.9)**                         | 3.5-3.8             | Ch 3 (7, 11, 13, 17)      |                                                              |
| 5    | 2/3/26   | **Compressibility, Homogeneity, Gradient (Ch 3.10-3.12)**            | Potentiometric Surface Mapping: Compute heads, interpolate grids, contour maps, flow direction                                 | **Class cancellation due to Winter Carnival**      | 3.10–3.12        | No Homework            |                                                              |
| 6    | 2/10/26  | **Darcy Flow in 2D (Ch 4.1–4.5)**             | Three-Point Gradient + Darcy Velocity: Compute gradients, q, v, anisotropy effects in Python                                   | **Anisotropy & Heterogeneity (Ch 4.6–4.9)**                 | 4.1–4.6         | Ch 4 (1, 3, 5, 7)        |                                                              |
| 7    | 2/17/26  | **Flow Nets (Ch 4.10-4.13)**                        | Digital Flow Nets: Laplace solver in Python; contouring potentials; flow net interpretation                                     | **Seepage Forces & Piping (Ch 4.14)**                    | 4.7–4.9         | Ch 4 (9, 11, 13, 15)     |                                                              |
| 8    | 2/24/26  | **MIDTERM**                                   | MIDTERM                                                                                                                       | **Exam Review**                                             | —               | —                       |                                                              |
| 9    | 3/3/26   | Spring Break (no class)                       | —                                                                                                                             | —                                                           | —               | —                       |                                                              |
| 10   | 3/10/26  | **Steady-State Wells (Ch 5.1–5.2)**           | Well Hydraulics: Fit Thiem equation using numpy, estimate T and K from pumping data                                            | **Specific Capacity & Transmissivity (Ch 5.3–5.4)**         | 5.1–5.4         | Ch 5 (1, 3, 5, 7)        | Project scope/narrative intro, 2–3 students/group  |
| 11   | 3/17/26  | **Theis Equation & Transient Flow (Ch 5.5–5.6)** | Theis Analysis: Implement W(u), curve fitting for T & S using scipy.special.expn                                              | **Cooper–Jacob Approximation (Ch 5.5–5.6)**                 | 5.5–5.6         | Ch 5 (9, 11, 13, 15)     |                                                              |
| 12   | 3/24/26  | **Regional Flow (Ch 6)**                      | FloPy: Regional Flow Model: Build Tóth basin concept, recharge, BCs, flow vectors; Introduce MODFLOW (FloPy): regional basin model | **Nested Flow Systems (Ch 6)**                              | 6               | Ch 6 (1, 3, 5, 7)        |                                                              |
| 13   | 3/31/26  | **Aquifer Testing (Ch 7)**                    | Full MODFLOW model: Build grids, parameters, BCs                                                                               | **Step-Drawdown Methods (Ch 7)**                           | 7               | Ch 7 (1, 3, 5, 9)        | ZOOM                                                         |
| 14   | 4/7/26   | **Groundwater Modeling Concepts (Ch 8): fracture flow & Karst** | Full MODFLOW (FloPy): Build grid, parameters, packages; water budgets; head visualization                                      | **Model Calibration (Ch 8)**                               | 8               | Ch 8 (1, 3, 7, 9)        |                                                              |
| 15   | 4/14/26  | **Review**                                     | Final Project Work Session: Students refine MODFLOW notebooks; instructor guidance                                             | Final Presentations                    | —               | —                       |                                                              |
| 16   | 4/21/26  | **FINAL EXAM**                                 | —                                                                                                                             | —                                                           | —               | —                       |                                                              |


---

## 🗓️ Important Dates (MTU Spring 2026)

* **Jan 5:** Instruction begins
* **Feb 4–8:** Winter Carnival Recess
* **Feb 28–Mar 8:** Spring Break
* **Apr 17:** Last day of regular instruction
* **Apr 20–24:** Final exam period

---

## 📝 Final Project

Students will design and simulate a conceptual groundwater system using **MODFLOW**. This project requires integrating aquifer parameters, boundary conditions, recharge/discharge zones, and transient responses.

Results will be presented in a **5–7 minute presentation** and a **short written report**.

---

## 📚 Course Policies

* **Attendance:** Regular attendance in both lecture and lab is expected. If needed, students may attend the lecture via Zoom. Please communicate with the instructor in advance to obtain the Zoom link.
* **Late Work:** Late assignments will be accepted up to 5 weekdays with a **2 points penalty per day**, unless an excuse is granted.
* **Academic Integrity:** Collaboration is encouraged on conceptual questions, but each student must submit their own original work.
* **Accessibility / Accommodations:** If you have a disability or need accommodations, please contact disability services and inform the instructor as soon as possible.
* **Lab Sessions:** Weekly 2-hour lab sessions are designed as **guided work time**. The TA will be present for the **entire lab period** to answer questions, assist with homework, and help troubleshoot coding or modeling exercises. Students are encouraged to use lab time to make progress on assignments and ask questions in real time.

---

## 📊 Grading Scale and Rounding Policy

Final course grades are calculated using a **100-point scale** and converted to letter grades and grade points as shown below. **Canvas displays numerical grades with decimals; however, letter grades are assigned using the rounded final score.**

### Rounding Policy

- The **final course average** is rounded to the **nearest whole number** before assigning a letter grade.
- **Standard rounding rules apply**:
  - Scores ending in **.5 or higher are rounded up**.
  - Scores ending below **.5 are rounded down**.

**Examples**

- 89.5 → 90 → **A**
- 84.5 → 85 → **AB**
- 79.5 → 80 → **B**
- 74.5 → 75 → **BC**
- 69.5 → 70 → **C**
- 64.5 → 65 → **CD**
- 59.5 → 60 → **D**

### Grade Conversion Table

| Rounded Final Score | Grade Points | Letter Grade |
|--------------------:|-------------:|--------------|
| 90–100 | 4.00 | A |
| 85–89  | 3.50 | AB |
| 80–84  | 3.00 | B |
| 75–79  | 2.50 | BC |
| 70–74  | 2.00 | C |
| 65–69  | 1.50 | CD |
| 60–64  | 1.00 | D |
| < 60   | 0.00 | F |

---

## ✨ Expected Outcomes

Students completing this course will be able to:

* Quantify aquifer and well parameters.
* Solve groundwater flow and transport problems using analytical and numerical tools.
* Interpret hydrogeologic and chemical data.
* Communicate groundwater analysis and modeling results effectively.
