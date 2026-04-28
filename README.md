# Tiny Core Linux: OS Installation & Kernel Analysis

## 📌 Overview
This project demonstrates the deployment of **Tiny Core Linux (CorePlus)** in a virtualized environment. It focuses on the efficiency of RAM-based execution and explores kernel-level operations through system call tracing.

## 🎯 Objectives
* **Frugal Installation:** Set up Tiny Core on an **ext4** filesystem via VirtualBox.
* **Kernel Analysis:** Use `strace` to capture and analyze the **`execve()`** system call.
* **Troubleshooting:** Resolve VM network isolation and repository access issues.

## 💻 Tech Stack
* **OS:** Tiny Core Linux (CorePlus)
* **Hypervisor:** Oracle VM VirtualBox
* **Filesystem:** ext4 (Journaling enabled)
* **Tools:** `strace`, `udhcpc`

## 🛠️ Key Steps
1. **VM Setup:** Allocated 512MB RAM and 2GB storage for optimal minimalist performance.
2. **Network Fix:** Restored connectivity using `sudo udhcpc` to allow extension downloads.
3. **System Call Trace:** Captured process execution data by running `strace ls`, verifying how the kernel handles binary execution.

## 🔍 Key Findings
* **Performance:** Running the OS from RAM eliminates disk I/O latency.
* **Kernel Insight:** Analysis of `execve` confirmed how the kernel manages process images and arguments.
* **Stability:** The ext4 filesystem provided robust data integrity during testing.

---
**Author:** Biruh Tesfa (BDU1701728)  
**Institution:** Bahir Dar University

