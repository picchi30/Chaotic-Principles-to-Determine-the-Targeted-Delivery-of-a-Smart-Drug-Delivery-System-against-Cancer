# Smart Drug Delivery System Simulation Using MATLAB Simulink

This repository contains a Simulink-based implementation of the mathematical model presented in the paper:

**"Insights on the Application of MATLAB and Chaotic Principles to Determine the Targeted Delivery of a Smart Drug Delivery System against Cancer in the Experimental Phase: A Prospective Approach"**  
Published in *Asian Journal of Pharmaceutics*, July-September 2020.

📄 [Link to Paper](https://www.researchgate.net/publication/343127347)

## 📌 Project Overview

The aim of this project is to simulate a **smart drug delivery system (SDDS)** that targets cancer cells using a combination of:

- **Nanoparticle-based drug delivery mechanisms**
- **Monoclonal antibody (MAB) targeting**
- **Chaotic dynamics modeling in cancer cell growth and treatment response**

The model leverages a **chaotic system of nonlinear differential equations**, representing:
- Healthy host cells
- Cancer cells
- Cells affected by targeted therapy

## 🧠 Core Model

The Simulink model is based on the chaotic system described in the paper, with equations of the form:

```
x1 = 0  
x2 = α(y − x)  
x3 = x(β − z) − y + γ  
x4 = δxy − z
```

Where:
- `x1`: Cancer cell density (starting from 0)  
- `x2`: Healthy host cells before cancer onset  
- `x3`: Malignant cell population  
- `x4`: Cells suppressed after drug targeting

Parameters used:
- α = 3.0  
- β = 26.5  
- γ = 0.74  
- δ = 0.5

## 🛠 Files Included

- `SDDS_Model.slx` – Simulink file simulating the chaotic cancer growth and suppression system  
- `README.md` – This file  
- (Optional) `figures/` – Folder with screenshots or simulation plots (phase portraits, time responses, etc.)  
- (Optional) `results/` – Folder to save your simulation outputs

## 🚀 How to Run

1. Open MATLAB.  
2. Navigate to the project directory.  
3. Open the Simulink file:
   ```matlab
   open('SDDS_Model.slx');
   ```
4. Run the simulation.  
5. View results in scope blocks or use `Simulink Data Inspector`.

## 📈 Expected Outputs

The simulation provides:
- **Chaotic behavior** of cancer cell dynamics  
- **Time response plots** showing interaction between healthy, cancerous, and suppressed cells  
- **Phase portraits** of system variables, illustrating non-linear dynamics

## 🔍 Future Work / To-Do

- Add control strategies (chaos control or feedback control)  
- Compare targeted vs non-targeted drug delivery systems  
- Add real patient-specific parameter adaptation for personalized simulation

## 📚 References

Moni, S.S., & Mohideen, B.N. (2020). *Insights on the Application of MATLAB and Chaotic Principles to Determine the Targeted Delivery of a Smart Drug Delivery System against Cancer in the Experimental Phase: A Prospective Approach*. Asian Journal of Pharmaceutics, 14(3), 319–329.  
[ResearchGate Link](https://www.researchgate.net/publication/343127347)

## 🙌 Acknowledgments

Inspired by the original work of Dr. Sivakumar S. Moni and Dr. Brem Navas.  
Special thanks to the Faculty of Pharmacy and College of Computer Science and IT, Jazan University.

---

*This simulation is intended for academic and research purposes only.*
