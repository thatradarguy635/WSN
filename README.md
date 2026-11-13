# WSN
A wireless sensor networks dashboard, aimed to simulate real world scenarios, using matlab as an app extension 
# Realistic WSN Telemetry, Channel & Spectrum Analytics Dashboard

An interactive, dark-themed **MATLAB App Designer** simulation and visualization suite for modeling Wireless Sensor Network (WSN) deployments under realistic RF propagation, MAC scheduling, traffic dynamics, and solar energy-harvesting conditions.

<img width="1598" height="926" alt="Screenshot 2026-11-13 154757" src="https://github.com/user-attachments/assets/36d5e55d-b688-4e7d-b246-ea1a8f4855d5" />
<img width="1598" height="927" alt="Screenshot 2026-11-13 154055" src="https://github.com/user-attachments/assets/88c5a667-92c6-4602-ad77-b89b5fc72a83" />

<img width="1597" height="922" alt="Screenshot 2026-11-13 154827" src="https://github.com/user-attachments/assets/a0680968-e8ad-41c3-9d2d-4c64611b5532" />

---

## Overview

Conventional WSN simulations often rely on idealized free-space channels and static battery drain models. **Realistic WSN Telemetry, Channel & Spectrum Analytics Dashboard** integrates physical-layer channel impairments, medium access control, event-driven traffic generation, and time-varying solar irradiance into a unified, single-screen engineering workbench. Users can sweep protocol and environmental parameters in real time, monitor network lifetime milestones, and export high-resolution figures directly from the interface.

---

## Key Features

### 1. Configurable Simulation Parameters

* **System, Channel & Protocol Configuration**
  * **RF & Link Budget:** Adjustable Channel Bandwidth (MHz), Transmit Power (dBm), Receiver Noise Figure (dB), and Rx Sensitivity (dBm).
  * **Propagation & Fading:** Configurable Path Loss Exponent, Log-Normal Shadowing Standard Deviation (dB) with Shadow Time-Correlation ($0\text{–}1$), and Small-Scale Fading profiles (e.g., Rician fading with selectable $K$-factor).
  * **Interference Modeling:** External interference occurrence probability and interference power floor (dBm).
* **MAC & Traffic Dynamics**
  * **Medium Access:** Selectable MAC protocols (such as TDMA Scheduled access), maximum retransmission limits, and payload sizing (up to 928 bits).
  * **Traffic Generation:** Configurable traffic models (e.g., Event-Driven Poisson), event arrival rates (events/round), and spatial event sensing radius (m).
* **Energy, Duty Cycle & Environment**
  * **Power & Harvesting:** Initial node battery energy (J), peak solar panel harvesting power (mW), radio duty cycle (%), and simulation start time of day (24-hour clock).
  * **Network Scale & Reliability:** Adjustable round duration (s), maximum simulation rounds, and random per-round hardware failure probability.

### 2. Eight-Tab Telemetry & Analytics Workspace

1. **Node Battery Levels:** Tracks residual energy trajectories and depletion patterns across individual sensor nodes.
2. **Channel & Spectrum Bandwidth:** Visualizes spectral occupancy, bandwidth efficiency, and channel capacity metrics.
3. **Executive Overview:** Summarizes high-level network health, throughput, and system performance indicators.
4. **Network Lifetime:** Plots active node count over simulation rounds and highlights **FND** (First Node Dead), **HND** (Half Nodes Dead), and **LND** (Last Node Dead).
5. **Latency & Delay:** Evaluates end-to-end packet delivery latency and retransmission delay distributions.
6. **Packet Delivery Ratio (PDR):** Monitors successful packet reception rates across varying channel and interference conditions.
7. **RSSI & Link Quality:** Analyzes received signal strength indicators, path loss attenuation, and link margin stability.
8. **Energy & Environment:** Displays a 2×2 diagnostic grid covering:
   * *Network Energy Consumption Breakdown (mJ/round)* split across **Control**, **Sensing + CPU**, **Sleep/Leak**, **Idle Listening**, **RX**, and **TX** states.
   * *Solar Irradiance Profile* modeling diurnal sun and cloud variations over simulation rounds.
   * *Energy Cost per Delivered Reading (mJ)* measuring energy efficiency per successful payload.
   * *Cluster-Head Duty per Node* tracking cluster-head role rotation balance across the network.

### 3. Built-In Execution & Figure Export

* **Live Status Telemetry:** Displays simulation completion progress alongside summary metrics (`PDR`, `FND`, `HND`, and `LND`).
* **One-Click Image Export:** Built-in **Export Image** control saves publication-ready dashboard snapshots directly from the app.


