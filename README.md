# Canteen_Credit_Management_system_s2-18_25-26


# 🍽️ Canteen Credit Management System

### Design of Digital Systems (DDS) Mini Project – 2025–26  
**Semester 2 | Team S2-18**

---

## 🔍 Abstract
This Verilog-based mini project implements a **Canteen Credit Management System** that manages students’ meal credits inside the college mess and canteen.  
Each student pays a fixed mess fee per semester and earns credits when they skip a meal.  
The collected credits can later be used to purchase snacks or food from the canteen.  
The system also calculates the additional cash required if the canteen amount exceeds available credits.

---

## 🎯 Objectives
- Track credits for **Breakfast, Lunch, Snacks, and Dinner**.  
- Provide **refund (credit add)** when a meal is skipped.  
- Allow students to **spend credits in the canteen**.  
- Display **remaining credits** and **extra cash needed** clearly.  
- Simulate and verify using **Verilog testbench**.

---

## 🧠 Features
- Designed using **Finite State Machine (FSM)** logic.  
- Supports both **refund** and **canteen deduction** operations.  
- Displays credits before and after each transaction.  
- Generates an `update_done` pulse for simulation output clarity.  
- Clean and fully self-contained — no external modules required.

---

## ⚙️ Files
| File | Description |
|------|--------------|
| `mess_credit_main.v` | Main Verilog module implementing the logic |
| `mess_credit_tb.v`   | Testbench that simulates 10 transactions |
| `mess_credit_wave.vcd` | (Generated) waveform file when run |

---

## ▶️ Run Instructions
To compile and simulate with **Icarus Verilog (iverilog)**:

```bash
iverilog -o mess_credit_sim mess_credit_main.v mess_credit_tb.v
vvp mess_credit_sim
