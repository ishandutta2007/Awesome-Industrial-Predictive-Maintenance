# Awesome-Industrial-Predictive-Maintenance

# Top Industrial Predictive Maintenance Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Condition Monitoring, Remaining Useful Life & Self-Hosted PdM Platforms*  
**Last updated: October 2026**

This repository tracks notable **commercial industrial predictive maintenance platforms** and **open-source projects** that monitor equipment health, detect early faults, and predict remaining useful life (RUL) — from fully managed cloud services to self-hosted frameworks for vibration analysis and anomaly detection.

**Examples** include Amazon Lookout for Equipment, Uptake, SparkCognition, C3 AI Predictive Maintenance, GE Digital APM, AVEVA Predictive Analytics, Augury, AspenTech Mtell, SymphonyAI Industrial, and Senseye (the category leaders).

**Open-source emphasis**: Industrial predictive maintenance is a strong open-source domain. **FD-REST** provides a lightweight, containerized REST platform for real-time fault detection with DNN inference and automated reporting . **Bearing-FDD** delivers explainable fault detection with MS2AE autoencoders, Dynamic Time Warping, and kurtogram-guided envelope analysis . **FaultSense** brings LSTM autoencoder anomaly detection with NASA CMAPSS benchmarks and a production REST API . **claude-stwinbox-diagnostics** bridges MEMS vibration sensors to LLMs via MCP for conversational fault diagnosis . **JOR 4.0** applies recursive Bayesian evidence fusion for vibration telemetry with ISO 20816-3 severity checks . **Vibrational Model Analysis** provides LSTM autoencoder anomaly detection for industrial bearings . **FluxStation** combines a 3D Digital Twin with Python-driven RUL prediction . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Amazon Lookout for Equipment](https://aws.amazon.com/lookout-for-equipment/)**  
  **AWS's managed predictive maintenance service** — uses machine learning to detect abnormal equipment behavior and predict failures . **Ingests sensor data from industrial equipment** without requiring ML expertise . **Best for AWS-native industrial monitoring** .

- **[C3 AI Predictive Maintenance](https://c3.ai/)**  
  **Enterprise AI application for predictive maintenance** — pre-built models and connectors for industrial assets . **Best for large-scale enterprise deployments** .

- **[GE Digital APM](https://www.ge.com/digital/applications/asset-performance-management)**  
  **Asset Performance Management platform** — predictive analytics, reliability, and maintenance optimization . **Best for industrial enterprises** .

- **[AVEVA Predictive Analytics](https://www.aveva.com/)**  
  **Predictive maintenance software** — early fault detection and RUL estimation for rotating equipment . **Best for process industries** .

- **[Augury](https://augury.com/)**  
  **Machine health platform** — vibration, temperature, and magnetic data with AI diagnosis . **Best for rotating equipment monitoring** .

- **[AspenTech Mtell](https://www.aspentech.com/)**  
  **Industrial AI platform** — predictive maintenance and anomaly detection for complex processes . **Best for process manufacturing** .

- **[SparkCognition](https://www.sparkcognition.com/)**  
  **AI-powered industrial analytics** — predictive maintenance and asset optimization . **Best for defense and industrial applications** .

- **[SymphonyAI Industrial](https://www.symphonyai.com/)**  
  **AI-driven predictive maintenance and asset performance** . **Best for industrial operations** .

- **[Uptake](https://www.uptake.com/)**  
  **Industrial AI platform** — predictive maintenance and asset reliability . **Best for heavy industry** .

- **[Senseye](https://www.senseye.io/)**  
  **Predictive maintenance platform** — automated condition monitoring and failure prediction . **Best for manufacturing and industrial equipment** .

## Open-Source GitHub Projects

### Fault Detection & Diagnosis Platforms

- **[FD-REST](https://github.com/Fraunhofer-IMS/FD-REST)**  
  **Lightweight RESTful platform for real-time fault detection and diagnosis in industrial systems**, open-source . **Integrates machine-learning-based fault detection into standard monitoring systems** . **Docker-based architecture with REST API** for on-premises deployment — maintains data security and integrity . **DNN-based inference** with user interface components for a complete predictive maintenance pipeline  . **Automated report generator** produces standardized summaries for benchmarking and maintenance planning . **Model-independent** — can be adjusted to alternative architectures . **Planned enhancements**: multi-asset tracking, MQTT/OPC-UA/Modbus compatibility, explainability modules, and playback features  . **Best for real-time industrial fault detection with on-prem deployment** .

- **[Bearing-FDD](https://github.com/paolocalderaro/bearing-fdd)**  
  **Early detection and diagnosis tool for bearing faults in rotating machinery**, open-source . **Explainable and interpretable fault detection** using Monotonic Smoothed Stacked Autoencoder (MS2AE) — trained on healthy data only, no faulty data required . **Multistage diagnostic procedure**: Dynamic Time Warping for baseline generation, kurtogram-guided bandpass filtering, Butterworth filtering, and envelope analysis for fault signature extraction  . **Determines fault type** (outer race, inner race, ball, cage) and **degradation stage** (early, medium, late) . **Web tool** with Java Spring frontend, Python REST API, and relational database . **Explainability reports** correlate Health Index (HI) with traditional time- and frequency-domain features . **Best for explainable bearing fault diagnosis** .

### Anomaly Detection & RUL Prediction

- **[FaultSense](https://github.com/momo-2609/faultsense)**  
  **LSTM autoencoder for anomaly detection and Remaining Useful Life prediction on NASA CMAPSS turbofan engine data**, open-source . **End-to-end deep learning pipeline** — reconstructs sensor windows to detect degradation, predicts RUL in cycles, and surfaces results through an interactive fleet health dashboard and REST API  . **Architecture**: encoder → latent space (dim=32) → decoder → RUL head . **Feature selection** from 21 sensors down to 14-15, min-max normalization per operating condition, sliding windows (seq_len=30) . **Results**: FD001 RMSE 14.85, NASA Score 311.6; FD003 RMSE 13.88, NASA Score 425.3 — beats Ridge baselines on every metric . **Production-ready REST API** with FastAPI and Plotly Dash dashboard . **MLflow logging** for experiment tracking . **Best for turbofan engine RUL prediction with production API** .

- **[JOR 4.0 Predictive Maintenance Fusion Engine](https://github.com/jamesorion6869/JOR_PYMC_V3_1)**  
  **Recursive Bayesian framework for industrial predictive maintenance with ISO 20816-3 compliance**, open-source research prototype  . **Weighted evidence fusion with recursive posterior updating** — produces non-healthy probability (NHP) estimate and hysteresis-controlled alert state . **Vibration telemetry converted to structured evidence** via ISO 20816-3 (Criterion I zone boundaries, Criterion II rate-of-change) . **Operational context grounded in NEMA MG-1** Class F thermal and load limits  . **Self-calibrating fusion engine** with validation tests for context stress, danger ramp, false-positive immunity, noise robustness, and long-duration stability  . **Domain-agnostic architecture** — replacing the evidence adapter while preserving the fusion engine demonstrates reusability . **Best for standards-based vibration severity monitoring** .

### Conversational & LLM-Integrated Diagnostics

- **[claude-stwinbox-diagnostics](https://github.com/LGDiMaggio/claude-stwinbox-diagnostics)**  
  **Open-source condition monitoring copilot and predictive maintenance AI agent**, open-source . **Connects industrial MEMS vibration sensors to Claude via MCP (Model Context Protocol)**  . **Transparent DSP pipeline** with standards-based severity checks (ISO 10816/20816) and conversational fault diagnosis . **Two MCP servers**: STWIN.box sensor acquisition and vibration analysis (FFT, envelope analysis, bearing fault detection) . **Three Claude Skills**: machine-vibration-monitoring, vibration-fault-diagnosis, operator-diagnostic-report  . **Supported fault types**: bearing inner/outer race, rolling element, cage, unbalance, misalignment, mechanical looseness  . **Hardware reference**: STEVAL-STWINBX1, but analysis server works with any vibration data source . **Status**: Proof of concept — full industrial validation in progress  . **Best for LLM-assisted condition monitoring** .

- **[Vibrational Model Analysis](https://github.com/matteo-martinelli/vibrational-model-analysis)**  
  **Deep Learning LSTM Autoencoder for vibrational anomaly detection and predictive maintenance in industrial bearings**, open-source . **Serves as baseline analytical engine for Cognitive Digital Twins**  . **Unsupervised anomaly detection** — reconstructs 4-sensor bearing signals; MAE > threshold (0.275) signifies mechanical degradation . **Pre-trained Keras/TensorFlow model (.h5)** and pre-fitted MinMaxScaler (.bin) included for immediate deployment  . **CLI inference pipeline** accepts JSON-formatted vibration data arrays . **Offline training and calibration** script with loss distribution plotting and threshold calculation . **Architecture**: Encoder (LSTM 16 → LSTM 4) → RepeatVector(1) → Decoder (LSTM 4 → LSTM 16 → TimeDistributed Dense) . **Best for unsupervised bearing anomaly detection** .

### Full-Stack IIoT Platforms

- **[FluxStation](https://github.com/FlaBingo/flux-station)**  
  **Full-stack IIoT platform with 3D Digital Twin and predictive maintenance**, open-source . **Real-time telemetry** from ESP32 sensors via WebSockets . **Interactive 3D Digital Twin** (React Three Fiber) reflecting temperature heat-maps and vibration movement  . **Predictive Analytics Engine** using Python (FastAPI, Pandas, Scikit-Learn) for anomaly detection and RUL calculation . **Multi-tenant SaaS architecture** with RBAC for managing independent machine fleets . **Industrial Health Dashboard** (Next.js, Shadcn/UI) with live charting and automated PDF maintenance reports . **Tech stack**: PostgreSQL, Drizzle ORM, Auth.js, Wokwi simulator . **Best for full-stack IIoT with digital twin** .

### Additional Strong Open-Source Options

- **MIHATT** — Multi-instance learning with HATT (Hoeffding Adaptive Tree) for weakly labeled sequential data, white-box interpretable fault detection with temporal locality  .
- **ECHO** — Frequency-aware hierarchical encoding for variable-length signals, state-of-the-art on SIREN benchmark for machine signal embeddings  .
- **Predictive-Maintenance-Industrial-IOT** (somjit101) — Statistical modelling and data visualization for failure analysis of boilers, pumps, motors (21 GitHub stars)  .
- **Predictive-Maintenance-using-LSTM** (umbertogriffo) — Multiple multivariate time series prediction with LSTM RNNs in Keras (640 GitHub stars)  .
- **FaultSense-LSTM** — Anomaly detection on NASA CMAPSS with interactive dashboard  .
- **awesome-predictive-maintenance** — Curated list of predictive maintenance research and repositories  .
- **mfg-predictive-maintenance** — Agent skill for designing PdM strategies using sensor data, RUL models, and P-F curve framework  .

**Frameworks for building custom industrial predictive maintenance solutions**: Combine **FD-REST** for lightweight, containerized real-time fault detection with REST API and on-prem deployment  . Use **Bearing-FDD** for explainable bearing fault diagnosis with MS2AE and DTW-based fault signature isolation  . Deploy **FaultSense** for turbofan RUL prediction with LSTM autoencoder and production API  . Integrate **JOR 4.0** for standards-based vibration severity monitoring with recursive Bayesian fusion  . Choose **claude-stwinbox-diagnostics** for LLM-assisted conversational fault diagnosis  . Use **FluxStation** for full-stack IIoT with 3D Digital Twin  . Note that true enterprise predictive maintenance with managed infrastructure, automated model training, and vendor-supported SLAs (Amazon Lookout for Equipment, C3 AI, GE Digital APM) remains primarily commercial territory; open-source stacks provide strong fault detection, RUL prediction, and condition monitoring foundations that require integration for complete industrial PdM deployments.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Industrial predictive maintenance platforms handle sensitive operational data and may influence critical maintenance decisions. Self-hosted solutions require proper security hardening, access controls, and compliance with industrial safety standards.
- **Open-source PdM projects vary significantly in maturity** — FD-REST and Bearing-FDD are production-oriented research tools ; claude-stwinbox-diagnostics is explicitly a proof of concept with full industrial validation still in progress  . Evaluate before relying on them for safety-critical maintenance decisions.
- **License considerations**: FD-REST is open-source ; Bearing-FDD is open-source ; FaultSense is open-source ; claude-stwinbox-diagnostics is open-source  . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong fault detection, RUL prediction, and condition monitoring foundations, but **managed infrastructure, automated model training, and vendor-supported SLAs** remain primarily commercial offerings.

---

**Made for maintenance engineers, reliability professionals, and organizations seeking predictive maintenance sovereignty.**  
Let's make industrial predictive maintenance more open, transparent, and proactive.
