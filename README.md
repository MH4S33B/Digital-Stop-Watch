# ⏱️ Digital Stopwatch Project – Digital Logic Design

A complete digital stopwatch designed using **Proteus 8.5** as part of a **Digital Logic Design (DLD)** course. This project demonstrates core concepts of digital electronics including **JK flip-flops**, **BCD counters**, **7-segment displays**, and a custom **1 Hz clock circuit** using the **555 Timer IC**.

---

## 🎯 Project Objectives

- ⏰ Display time in HH:MM:SS format using six 7-segment displays.
- 🔄 Implement BCD counters for hours, minutes, and seconds.
- 🧮 Design custom reset and start/stop logic using logic gates.
- 🧪 Simulate and test the design thoroughly in Proteus 8.5.

---

## 💡 Features

- ✅ Hour, minute, and second counters using JK Flip-Flops
- ✅ Reset logic to return to 00:00:00
- ✅ Start/Stop control using enable signal
- ✅ Custom-built 1 Hz clock using 555 Timer
- ✅ Realistic 24-hour time cycle (00:00:00 → 23:59:59)

---

## ⚙️ Components Used

- **JK Flip-Flops** (7473 Dual Flip-Flop ICs)
- **BCD to 7-Segment Decoders** (7447)
- **7-Segment Displays**
- **Logic Gates** (AND, NAND)
- **555 Timer IC** (for custom 1 Hz clock)
- **Resistors, Capacitors** (for timing and logic support)

---

## 🧰 Tools & Software

- 🖥️ **Proteus 8.5** (Simulation & Design)
- 📝 **Manual Calculations** for timer frequency
- ⚙️ **Digital Logic Theory** for design planning

---

## 📐 Circuit Overview

### 🧮 Time Display Modules
| Unit | Range | Description |
|------|-------|-------------|
| **S1** | 0-9 | Seconds (Units) |
| **S2** | 0-5 | Seconds (Tens) |
| **M1** | 0-9 | Minutes (Units) |
| **M2** | 0-5 | Minutes (Tens) |
| **H1** | 0-9 | Hours (Units) |
| **H2** | 0-2 | Hours (Tens, 24hr format) |

Each is implemented with:
- **JK Flip-Flops** for counting
- **BCD to 7-Segment decoder**
- **Carry logic** for triggering the next stage

### 🔁 Reset Logic
- Manual or auto-reset on reaching 24:00:00
- Uses **NAND gates** to drive CLR inputs on all flip-flops

### ⏯️ Clock Control
- Uses an **AND gate** to gate the 1 Hz clock signal
- External toggle signal controls start/stop behavior

### ⏲️ Clock Circuit (1 Hz)
- Built using **555 Timer IC** in **astable mode**
- Component values: `R1 = 10kΩ`, `R2 = 10kΩ`, `C1 = 47µF`
- Generates clean square wave to drive counters

---

## 📸 Screenshots
<p align="center"> <img src="https://github.com/MH4S33B/Digital-Stop-Watch/blob/main/Pictures/Complete%20Stopwatch.png" alt="Circuit Diagram" width="400"> </p>
<p align="center"> <img src="https://github.com/MH4S33B/Digital-Stop-Watch/blob/main/Pictures/Ones%20of%20Hour.jpg" alt="Circuit Diagram" width="400"> </p>
<p align="center"> <img src="https://github.com/MH4S33B/Digital-Stop-Watch/blob/main/Pictures/Clock.jpg" alt="Circuit Diagram" width="400"> </p>


## 📁 Project Files
```
Stopwatch-Project/
├── Circuit Diagram Proteus 8.5.pdsprj
├── Project Report.pdf
├── README.md
└── Pictures
```


---

## 🧪 Use Cases

- 🎓 Educational DLD or Embedded Systems Labs
- 🔍 Logic Design Demonstration
- 🔧 Simulation Practice with Proteus
- 📚 Foundational exposure to digital clock architecture

---

## 🛡️ Disclaimer

This project is for **educational purposes only**. Please do not deploy in real-time or production environments without proper enhancements.

---

## 🤝 Authors & Contributors

- Muhammad Haseeb – `242292`
- Ahmed Saleem – `242348`  
- Syed Ahtsham Hussain Shah – `242364`  
- Haroon Ul Haq – `240692`    

Project developed as part of the **Digital Logic Design** course at <a href="https://www.au.edu.pk/">Air University</a>.

---

## ⭐ GitHub

If you found this project helpful, give it a ⭐ and consider contributing!

---

## 📬 Contact

For feedback, questions, or collaboration:

- 💻 GitHub: [MH4S33B](https://github.com/MH4S33B)
- ✉️ Email: mhaseebraja2006@gmail.com
- 💼 LinkedIn: [linkedin.com/in/mhaseeb211](https://www.linkedin.com/in/mhaseeb211)
- 📝 Medium: [@mh4s33b](https://medium.com/@mh4s33b)
