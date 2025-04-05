# 5-stage-ring-oscillator
Simulation and analysis of a 5-stage CMOS ring oscillator using Cadence Virtuoso
# 5-Stage CMOS Ring Oscillator

This project demonstrates the design, simulation, and analysis of a 5-stage ring oscillator using **Cadence Virtuoso** and **Spectre Simulator**.

## 🔧 Tools Used
- Cadence Virtuoso (ADE L)
- Spectre for simulation
- GPDK 90nm PDK

## 🧠 Objective
To design a 5-stage CMOS ring oscillator and analyze the frequency variation using **parametric sweep** of capacitance.

## 📂 Project Structure
- `schematic/` – Circuit diagram
- `waveforms/` – Transient and parametric waveform outputs
- `results/` – Notes on frequency, voltage levels, delay, etc.
- `docs/` – In-depth explanation and methodology

## 📈 Parametric Analysis
Capacitor `C_var` is varied to observe its effect on oscillation frequency. The output shows a clear inverse relationship between capacitance and frequency.

## 📷 Screenshots
### Schematic
![Schematic](schematic/fivestageringoscillator.png)

### Parametric Sweep
![Parametric](waveforms/Parametric_5r.png)

---

## 🧪 Sim Results (Summary)
| Capacitance (pF) | Frequency (MHz) |
|------------------|-----------------|
| 0.01             | 99.2            |
| 0.05             | 42.3            |
| 0.1              | 28.5            |

---

## 📜 License
This project is licensed under the MIT License.
