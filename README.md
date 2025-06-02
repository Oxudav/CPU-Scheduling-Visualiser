# 🧠 CPU Scheduling Algorithm Visualiser

Visualize and compare 9 CPU scheduling algorithms using Gantt charts, performance metrics, and animations.

🔗 [GitHub Repo](https://github.com/Oxudav/CPU-Scheduling-Visualiser)

---

## 📌 About

CPU scheduling algorithms decide the order in which processes access the CPU. This tool helps you understand how each algorithm works and compare their performance in real-time.

---

## 🚀 Features

- Gantt chart + animation for each algorithm
- Avg turnaround time & waiting time display
- Highlights the best algorithm using a ranking system
- Toggle & compare multiple algorithms
- Includes a new hybrid algorithm (Round Robin + SJF + Priority)

---

## ⚙️ Supported Algorithms

1. FCFS  
2. SJF (Non-preemptive & Preemptive)  
3. LJF (Non-preemptive & Preemptive)  
4. Round Robin  
5. Priority (Non-preemptive & Preemptive)  
6. **Hybrid Algorithm** (custom implementation)

---

## 🖥️ How to Use

1. Add/Edit/Delete processes in the table  
2. Click **Evaluate** to compare algorithms  
3. Click **Visualise** to see animations

Each process includes:
- Process ID (auto-assigned)
- Burst Time
- Arrival Time
- Priority

---

## 🧪 Hybrid Algorithm Logic

A custom algorithm combining SJF, Priority, and Round Robin:

1. Assume all processes arrive at time 0  
2. Calculate time quantum:  
   `TQ = √[(Σ Burst Time × Max Burst Time) / Number of Processes]`  
3. Rank based on burst time and priority  
4. Compute adjusted priority:  
   `Adjusted = ¾ × Priority Rank + ¼ × Burst Time Rank`  
5. Execute with Round Robin using the new queue and TQ

📄 [Research Reference](https://www.researchgate.net/publication/49619229_An_Improved_Round_Robin_Schedduling_Algorithm_for_CPU_Scheduling)

---

## 📂 Source Code

🔗 [GitHub - mukul2310/cpu-scheduler-visualiser](https://github.com/Oxudav/CPU-Scheduling-Visualiser)

---

## 🙌 Thanks for visiting!
