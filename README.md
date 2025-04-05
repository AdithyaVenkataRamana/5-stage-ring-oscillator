# 🔁 5-Stage CMOS Ring Oscillator using Cadence Virtuoso

---

## 🧾 Abstract

This project presents the design and simulation of a **5-stage CMOS ring oscillator** using **Cadence Virtuoso**. The oscillator is built with five inverter stages connected in a loop to generate a periodic output without an external clock. The objective is to analyze the delay, frequency, and stability of oscillations through transistor-level simulations and parametric analysis. The project aims to contribute toward understanding the timing behavior and performance of ring oscillators, which are widely used in clock generation and delay circuits in VLSI design.

---

## 1. Introduction

A ring oscillator is a simple, yet essential building block in digital and analog circuits. It consists of an odd number of inverter stages connected in a feedback loop. The delay introduced by each stage contributes to the total oscillation period. Ring oscillators are often used for on-chip clock generation, PVT (process-voltage-temperature) monitoring, and performance characterization in VLSI circuits.

This project focuses on implementing a **5-stage ring oscillator**, extending the conventional 3-stage design to study the effects of increased delay and its impact on oscillation frequency.

---

## 2. Background

Ring oscillators rely on the principle that an odd number of inverters in a loop will produce an unstable system, resulting in continuous transitions — essentially forming a square wave oscillator. The oscillation frequency is primarily determined by:

- Number of inverter stages (N)
- Propagation delay of each stage (tp)

The fundamental frequency of a ring oscillator can be estimated as:


Increasing the number of stages or the delay per stage decreases the oscillation frequency. Cadence Virtuoso allows for detailed modeling of this behavior using CMOS transistor-level schematics and simulation tools.

---

## 3. Design Methodology

The design was implemented and simulated using the following steps:

- **CMOS Inverter Design:** A standard CMOS inverter was designed using nMOS and pMOS transistors with typical W/L ratios.
- **5-Stage Ring Configuration:** Five such inverters were connected in series with the output of the fifth stage fed back to the input of the first.
- **Biasing and Power:** The circuit was powered using VDD = 1.8V, with all inverter stages uniformly biased.
- **Transient Simulation:** The output waveform was captured over time to observe stable oscillation.
- **Parametric Analysis:** Delay and load variations were introduced to observe their effect on frequency.

Tools used:
- **Cadence Virtuoso Schematic Editor**
- **Analog Design Environment (ADE) for simulation**

---

## 4. Simulation and Results

Several simulation snapshots were obtained to validate the design:

- **Transient Analysis:**Transient analysis is employed to see the time-domain output of the ring oscillator. In this 5-stage CMOS ring oscillator, the transient response illustrates a periodic oscillation due to propagation delay across every inverter stage. When simulated, the output waveform illustrates a stable and repeatable oscillation, which confirms the self-sustaining characteristic of the ring oscillator.

As observed in the simulation result, the output voltage alternates between high and low levels with a regular period. This verifies the intended operation of the ring oscillator, in which the feedback loop makes the signal invert and move continuously, resulting in an oscillating waveform. The frequency of oscillation relies on the number of stages and the delay per stage, depending on the load capacitance and transistor size.

The temporary plot indicates definite periodic waveforms for the delay through each of the 5 inverters within the loop, and the waveform remains consistent with time.
- **Parametric Sweep:**
  - Delay and frequency were analyzed as design parameters (W/L ratios, capacitance, etc.) were varied.

📂 Key Simulation Files:
- `Fring.png` — Transient waveform showing steady oscillation.
- `P2-5r.png` — Delay characterization across time.
- `Parametric_5r.png` — Frequency variation with changing parameters.

---

## 5. Conclusion

The design and simulation of a **5-stage CMOS ring oscillator** were successfully completed using Cadence Virtuoso. Compared to simpler 3-stage oscillators, the 5-stage configuration offers deeper insights into timing behavior and allows fine-grained frequency tuning. The results confirm the theoretical relationship between delay, number of stages, and frequency, validating the design’s correctness and stability.

This implementation can serve as a foundation for further exploration in VLSI clock generation, delay-based sensors, and frequency calibration techniques.

---

## 📌 Reference

🎥 [YouTube: CMOS Ring Oscillator in Cadence Virtuoso](https://youtu.be/t5emusIwI70?si=rJy2WCOhYKEpj8B4)

---

## 👨‍💻 Author

**Adithya Venkata Ramana**  
VLSI Design Enthusiast | Cadence | Digital & Analog Simulation

---

## 📜 License

This project is released for educational and non-commercial use. Attribution is appreciated.
