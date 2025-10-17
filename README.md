# CASE-STUDY-

Case Study Title: Resource Allocation and Cost Optimization in an OpenStack Private Cloud

Case Overview:

ABC Cloud Services runs a private cloud using OpenStack to host virtual machines (VMs) for internal development, testing, and production workloads. Their cloud infrastructure comprises:

5 Compute Nodes, each with:
64 vCPUs
256 GB RAM
2 TB SSD storage
OpenStack Services Deployed:
Nova (Compute)
Neutron (Networking)
Cinder (Block Storage)
Glance (Image Management)
Keystone (Identity)
Horizon (Dashboard)
Heat (Orchestration)

They are considering expanding their cloud but want to first evaluate current capacity usage, VM density, and cost efficiency. The goal is to calculate whether their resource usage aligns with business needs and how to optimize it.

Case Study Questions – OpenStack Calculation in Cloud Computing

1. Resource Utilization:

Based on the current infrastructure, what is the total available compute capacity in terms of:
Total vCPUs
Total RAM
Total storage

2.Storage Allocation:

Given 10 TB of total block storage across the cloud, how many VMs can be supported if:
a) Each VM is allocated 100 GB block storage
b) Snapshot storage consumes 20% extra on average

**SOLUTIONS:**

---

## Case Study: Cloud Performance and Efficiency Analysis

### 1. Introduction

Cloud computing is central to modern IT operations, but system effectiveness depends heavily on performance and resource efficiency. Key factors—encryption speed, CPU utilization, network performance, power consumption, and VM allocation—directly affect cost, productivity, and sustainability. This case study analyzes five real-world scenarios to measure and interpret cloud efficiency.

---

### 2. Background

Organizations relying on cloud services often face challenges like:

* Encrypting large volumes of data efficiently
* Balancing CPU workloads
* Optimizing network throughput
* Minimizing energy consumption
* Ensuring optimal VM distribution

Measuring these metrics allows better resource allocation, cost reduction, and performance improvement.

---

### 3. Case Analyses

#### **Case 1: Encryption Time for Data Upload**

* **Scenario:** Encrypting 2 TB using AES-256 at 0.05 s/MB
* **Calculation:**
  [
  2,\text{TB} = 2 \times 1024 \times 1024 = 2{,}097{,}152,\text{MB}
  \text{Time} = 2{,}097{,}152 \times 0.05 = 104{,}857.6,\text{s} \approx 29.13,\text{hours}
  ]
* **Result:** ~29 hours required
* **Insight:** Security comes at a significant time cost for large-scale data transfers.

---

#### **Case 2: CPU Utilization Efficiency**

* **Scenario:** VM has 8 vCPUs, average usage 5.5 vCPUs
* **Calculation:**
  [
  \text{Efficiency} = \frac{5.5}{8} \times 100 = 68.75%
  ]
* **Result:** 68.75% CPU utilization
* **Insight:** One-third of CPU resources are unused, indicating potential for downsizing to save costs.

---

#### **Case 3: Network Throughput Efficiency**

* **Scenario:** 1 Gbps bandwidth, achieves 600 Mbps peak
* **Calculation:**
  [
  \text{Throughput Efficiency} = \frac{600}{1000} \times 100 = 60%
  ]
* **Result:** 60% efficiency
* **Insight:** 40% of bandwidth unused; optimizations may improve network performance.

---

#### **Case 4: Energy Efficiency Comparison**

* **Scenario:** Two setups performing same workload

  * Setup A: 500 W × 2 h = 1.0 kWh
  * Setup B: 300 W × 3.5 h = 1.05 kWh
* **Result:** Setup A slightly more energy-efficient
* **Insight:** Lower power consumption doesn’t guarantee efficiency; total energy = power × time.

---

#### **Case 5: Maximum Efficient VM Allocation**

* **Scenario:** Server has 16 CPU cores; each VM needs 2 cores; max 75% CPU utilization
* **Calculation:**
  [
  \text{Usable cores} = 16 \times 0.75 = 12
  \text{Max VMs} = 12 \div 2 = 6
  ]
* **Result:** 6 VMs
* **Insight:** Over-provisioning VMs can degrade performance; controlled allocation ensures stability.

---

### 4. Discussion

* **Encryption:** Long delays affect upload speed; trade-off between security and performance
* **CPU Utilization:** Underused resources increase cost; resizing VMs can improve efficiency
* **Network:** Bandwidth inefficiencies impact user experience; network optimization is crucial
* **Energy:** Small differences in setup power/time can affect sustainability
* **VM Allocation:** Proper CPU-based VM limits prevent performance degradation

**Key Takeaway:** Simple calculations and monitoring guide smarter cloud resource management, balancing cost, performance, and energy efficiency.

---

### 5. Conclusion

Efficient cloud operations require evaluating multiple metrics. Insights from the five scenarios:

| Metric             | Formula Used       | Result                    | Key Insight                          |
| ------------------ | ------------------ | ------------------------- | ------------------------------------ |
| Encryption Time    | 0.05 s/MB × 2 TB   | 29.1 h                    | Encryption adds delay for large data |
| CPU Efficiency     | (5.5 ÷ 8) × 100    | 68.75%                    | CPU underutilized                    |
| Network Efficiency | (600 ÷ 1000) × 100 | 60%                       | Bandwidth underused                  |
| Energy Efficiency  | Power × Time       | A = 1.0 kWh, B = 1.05 kWh | Setup A better                       |
| VM Allocation      | (16 × 0.75) ÷ 2    | 6 VMs                     | Stable load maintained               |

---
