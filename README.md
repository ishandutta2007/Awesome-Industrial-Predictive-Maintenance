<p align="center">
  <img src="assets/banner.svg" alt="Awesome Industrial Predictive Maintenance Banner" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Industrial-Predictive-Maintenance/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Industrial-Predictive-Maintenance?style=flat-square&logo=github" alt="GitHub_Stars"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Industrial-Predictive-Maintenance/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Industrial-Predictive-Maintenance?style=flat-square&logo=github" alt="GitHub forks"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Industrial-Predictive-Maintenance/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Industrial-Predictive-Maintenance?style=flat-square" alt="License"/></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

# ⚙️ Awesome Industrial Predictive Maintenance

## 🏭 Top Industrial Predictive Maintenance Ecosystem (PdM & IIoT)

**Curated List of Commercial SaaS Products & Open-Source GitHub Projects**  
*Focused on Condition Monitoring, Remaining Useful Life (RUL) Prediction, Machinery Fault Diagnosis & IIoT Analytics*  

📅 **Last updated: October 2026**

---

### 📌 Overview
This repository provides a comprehensive, research-grade directory of **commercial industrial predictive maintenance (PdM) platforms** and **open-source machine learning frameworks**. These tools enable maintenance engineers, reliability specialists, and data scientists to monitor machinery health, detect early mechanical anomalies, diagnose bearing/gearbox degradation, and compute Remaining Useful Life (RUL) from high-frequency sensor telemetry (vibration, acoustic emission, temperature, and current).

---

## 📑 Table of Contents
- [📊 Sector Market Overview](#-sector-market-overview)
- [🏭 SaaS & Commercial Platforms](#-saas--commercial-platforms)
- [🔓 Open-Source GitHub Repositories (Ranked by Stars)](#-open-source-github-repositories-ranked-by-stars)
- [🛠️ Architectural Guidance & Integration Stacks](#️-architectural-guidance--integration-stacks)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [📈 Star History](#-star-history)
- [📝 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer](#-disclaimer)

---

## 📊 Sector Market Overview

> 💡 **Market Dynamics**: The global industrial predictive maintenance market is valued at **$10B–$20B in 2026** and projected to exceed **$60B–$200B+ by 2033–2035 (CAGR ~25–30%)**. The market is **moderately to highly fragmented** (top 5 vendors hold ~32–38% market share) rather than a winner-take-all ecosystem. This fragmentation is driven by domain specificity across diverse asset classes (rotating equipment, turbomachinery, process pumps), complex edge/on-prem integration requirements, and heterogeneous OEM sensor interfaces.

---

## 🏭 SaaS & Commercial Platforms

The following enterprise platforms offer managed cloud infrastructure, automated model training, pre-built asset models, and vendor SLAs. They are sorted in **descending order by company size (Valuation / Market Cap / Revenue)**:

| Product / Platform | Company Size (Valuation / Revenue) 📈 | Specific Starting Pricing 💵 | Free Tier / Free Trial Limit 🎁 | Target Use Case & Key Strengths 🎯 |
| :--- | :--- | :--- | :--- | :--- |
| **[Amazon Lookout for Equipment](https://aws.amazon.com/lookout-for-equipment/)** | **$2.0 Trillion** Market Cap (AWS parent; ~$90B+ AWS Rev.) | **$0.10/GB** data ingestion + **$0.75/hr** model training + **$0.25/metric-hr** inference | **1st month free trial** (up to 50 GB ingestion, 250 training hours, 168 hours scheduled inference) | AWS-native ML anomaly detection for industrial equipment sensor streams |
| **[Senseye](https://www.senseye.io/)** | **$150 Billion** Market Cap (Siemens AG parent; ~$85B Rev.) | **~$1,500 / month** (~$18,000/yr base coverage for 20 assets) | **30-day proof-of-concept trial** (up to 10 connected telemetry sensor streams) | Automated condition monitoring for manufacturing equipment fleets |
| **[AVEVA Predictive Analytics](https://www.aveva.com/)** | **$140 Billion** Market Cap (Schneider Electric parent; ~$38B Rev.) | **~$2,500 / month** (~$30,000/yr entry AVEVA Connect subscription) | **30-day free trial** on AVEVA Connect (limited to 5 rotating equipment models) | Early fault detection & RUL estimation for process industries |
| **[GE Digital APM](https://www.ge.com/digital/applications/asset-performance-management)** | **$75 Billion** Market Cap (GE Vernova parent; ~$35B Rev.) | **~$10,000 / month** (~$120,000/yr enterprise base node deployment) | **30-day interactive sandbox trial** (up to 5 simulated asset models & sample telemetry) | Enterprise asset performance management for energy and heavy industry |
| **[AspenTech Mtell](https://www.aspentech.com/)** | **$65 Billion** Market Cap (Emerson Electric parent; ~$17B Rev.) | **~$2,500 / month** (~$30,000/yr starting aspenOne license) | **30-day evaluation sandbox trial** (pre-loaded process data & model builder sandbox) | Pattern-recognition anomaly detection for continuous process manufacturing |
| **[C3 AI Predictive Maintenance](https://c3.ai/)** | **$1.75 Billion** Market Cap (NYSE: AI; ~$310M Rev.) | **$0.55 / vCPU-hour** (AWS Marketplace pay-as-you-go; ~$250k/yr enterprise contract) | **14-day free trial** on C3 AI Studio (1 workspace & sample operational datasets) | Pre-built enterprise AI applications for defense & large manufacturing fleets |
| **[SparkCognition](https://www.sparkcognition.com/)** | **$1.4 Billion** Valuation (Privately held Unicorn; ~$50M+ Rev.) | **~$4,000 / month** (~$48,000/yr baseline enterprise contract) | **30-day enterprise sandbox trial** (1 streaming data pipeline, up to 5 asset nodes) | AI-powered analytics for defense, energy, and industrial asset optimization |
| **[Augury](https://augury.com/)** | **$1.2 Billion** Valuation (Privately held Unicorn; ~$155M Rev.) | **~$1,500 / month** (~$18,000/yr hardware + SaaS bundle for ~10 assets) | **30-day risk-free pilot trial** (up to 4 machine trains with hardware installed) | End-to-end machine health platform for rotating equipment |
| **[SymphonyAI Industrial](https://www.symphonyai.com/)** | **$1.0 Billion** Valuation (Privately held; ~$100M+ Rev.) | **~$1,666 / month** (~$20,000/yr starting SaaS platform) | **30-day guided sandbox trial** (3 machine profiles & 100 hours signal ingestion) | Industrial AI asset performance and predictive maintenance workflows |
| **[Uptake](https://www.uptake.com/)** | **$1.0 Billion** Valuation (Privately held Unicorn; ~$45M Rev.) | **~$1,250 / month** (~$15,000/yr per site baseline tier) | **14-day free trial** (pre-loaded fleet telemetry datasets and anomaly dashboards) | Heavy industry asset reliability and failure prevention analytics |

---

## 🔓 Open-Source GitHub Repositories (Ranked by Stars)

The open-source domain provides analytical libraries, deep learning architectures, Bayesian fusion engines, and full-stack IIoT platforms. Sorted in **descending order by GitHub_Stars_Count**:

- **[PyOD (Python Outlier Detection)](https://github.com/yzhao062/pyod)** [![GitHub_Stars](https://img.shields.io/github/stars/yzhao062/pyod?style=social&color=white)](https://github.com/yzhao062/pyod/stargazers) — Comprehensive Python toolkit for detecting anomalies and outliers in industrial multivariate sensor telemetry. Includes 40+ algorithms (Autoencoders, Isolation Forests, VAEs, PCA) tailored for machine fault detection.
- **[sktime](https://github.com/sktime/sktime)** [![GitHub_Stars](https://img.shields.io/github/stars/sktime/sktime?style=social&color=white)](https://github.com/sktime/sktime/stargazers) — Unified machine learning framework for time series analysis, telemetry forecasting, and industrial sensor anomaly classification.
- **[lifelines](https://github.com/camdavidsonpilon/lifelines)** [![GitHub_Stars](https://img.shields.io/github/stars/camdavidsonpilon/lifelines?style=social&color=white)](https://github.com/camdavidsonpilon/lifelines/stargazers) — Survival analysis library in Python, widely used for modeling component survival probability, failure hazards, and Remaining Useful Life (RUL) curves.
- **[Predictive-Maintenance-using-LSTM](https://github.com/umbertogriffo/Predictive-Maintenance-using-LSTM)** [![GitHub_Stars](https://img.shields.io/github/stars/umbertogriffo/Predictive-Maintenance-using-LSTM?style=social&color=white)](https://github.com/umbertogriffo/Predictive-Maintenance-using-LSTM/stargazers) — Deep learning implementation in Keras/TensorFlow for multivariate time-series prediction and RUL estimation using the NASA CMAPSS jet engine degradation benchmark.
- **[awesome-predictive-maintenance](https://github.com/vincent-zurczak/awesome-predictive-maintenance)** [![GitHub_Stars](https://img.shields.io/github/stars/vincent-zurczak/awesome-predictive-maintenance?style=social&color=white)](https://github.com/vincent-zurczak/awesome-predictive-maintenance/stargazers) — Curated collection of predictive maintenance research papers, benchmark datasets, and analytical tools.
- **[FD-REST](https://github.com/Fraunhofer-IMS/FD-REST)** [![GitHub_Stars](https://img.shields.io/github/stars/Fraunhofer-IMS/FD-REST?style=social&color=white)](https://github.com/Fraunhofer-IMS/FD-REST/stargazers) — Lightweight RESTful platform for real-time fault detection and diagnosis with Docker-based on-premise deployment, DNN inference, and automated PDF maintenance reporting.
- **[Predictive-Maintenance-Industrial-IOT](https://github.com/somjit101/Predictive-Maintenance-Industrial-IOT)** [![GitHub_Stars](https://img.shields.io/github/stars/somjit101/Predictive-Maintenance-Industrial-IOT?style=social&color=white)](https://github.com/somjit101/Predictive-Maintenance-Industrial-IOT/stargazers) — Statistical modeling, exploratory data analysis, and failure visualization for industrial boilers, pumps, and electric motors.
- **[Bearing-FDD](https://github.com/paolocalderaro/bearing-fdd)** [![GitHub_Stars](https://img.shields.io/github/stars/paolocalderaro/bearing-fdd?style=social&color=white)](https://github.com/paolocalderaro/bearing-fdd/stargazers) — Explainable bearing fault diagnosis using Monotonic Smoothed Stacked Autoencoders (MS2AE), Dynamic Time Warping (DTW), kurtogram bandpass filtering, and envelope analysis.
- **[FaultSense](https://github.com/momo-2609/faultsense)** [![GitHub_Stars](https://img.shields.io/github/stars/momo-2609/faultsense?style=social&color=white)](https://github.com/momo-2609/faultsense/stargazers) — End-to-end deep learning pipeline featuring an LSTM autoencoder for anomaly detection and turbofan engine RUL prediction with FastAPI REST API & Plotly Dash dashboard.
- **[claude-stwinbox-diagnostics](https://github.com/LGDiMaggio/claude-stwinbox-diagnostics)** [![GitHub_Stars](https://img.shields.io/github/stars/LGDiMaggio/claude-stwinbox-diagnostics?style=social&color=white)](https://github.com/LGDiMaggio/claude-stwinbox-diagnostics/stargazers) — Conversational condition monitoring copilot connecting industrial MEMS vibration sensors (STEVAL-STWINBX1) to Claude via Model Context Protocol (MCP) with ISO 10816/20816 severity checks.
- **[JOR 4.0 Predictive Maintenance Fusion Engine](https://github.com/jamesorion6869/JOR_PYMC_V3_1)** [![GitHub_Stars](https://img.shields.io/github/stars/jamesorion6869/JOR_PYMC_V3_1?style=social&color=white)](https://github.com/jamesorion6869/JOR_PYMC_V3_1/stargazers) — Recursive Bayesian evidence fusion engine adhering to ISO 20816-3 vibration severity standards and NEMA MG-1 Class F thermal/load limits.
- **[Vibrational Model Analysis](https://github.com/matteo-martinelli/vibrational-model-analysis)** [![GitHub_Stars](https://img.shields.io/github/stars/matteo-martinelli/vibrational-model-analysis?style=social&color=white)](https://github.com/matteo-martinelli/vibrational-model-analysis/stargazers) — Unsupervised LSTM Autoencoder baseline for vibrational anomaly detection in industrial bearings, serving as an analytical engine for Cognitive Digital Twins.
- **[FluxStation](https://github.com/FlaBingo/flux-station)** [![GitHub_Stars](https://img.shields.io/github/stars/FlaBingo/flux-station?style=social&color=white)](https://github.com/FlaBingo/flux-station/stargazers) — Full-stack IIoT platform featuring an interactive 3D Digital Twin (React Three Fiber), WebSockets ESP32 telemetry, and Python-driven RUL calculation engine.

---

## 🛠️ Architectural Guidance & Integration Stacks

Organizations building self-sovereign or hybrid predictive maintenance infrastructure can integrate open-source building blocks:
- 🔌 **Ingestion & Protocol Bridging**: Use **FluxStation** for MQTT/WebSocket sensor acquisition from edge hardware.
- ⚡ **Real-Time Fault Detection**: Deploy **FD-REST** for containerized RESTful DNN inference or **PyOD** for multivariate outlier evaluation.
- 🩺 **Signal Processing & Feature Extraction**: Apply **Bearing-FDD** for envelope analysis and Dynamic Time Warping (DTW) on vibration signals.
- 🧠 **Standards Compliance & Decision Fusion**: Integrate **JOR 4.0** for recursive Bayesian posterior updates compliant with ISO 20816-3.
- 🤖 **LLM Diagnostics Copilot**: Connect **claude-stwinbox-diagnostics** via MCP for natural language diagnostic reporting.

---

## 💖 Support & Sponsorship

Thank you for visiting **Awesome Industrial Predictive Maintenance**! If this curated list has saved you engineering hours, supported your research, or guided your industrial IoT deployments:

- ⭐ **Star this repository** on GitHub to increase its visibility.
- 🔀 **Fork & Share** it with reliability engineers, asset managers, and AI practitioners.
- ☕ **Sponsor the Maintainer**: Support ongoing curation and maintenance via the [GitHub Sponsors Dashboard](https://github.com/sponsors/ishandutta2007).

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Industrial-Predictive-Maintenance&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Industrial-Predictive-Maintenance&type=date&legend=top-left)

---

## 📝 How to Contribute

1. 🍴 Fork this repository.
2. ✏️ Add or update entries in `README.md` following the established table / list format.
3. 🔗 Ensure all links, pricing details, and Stars_Badges are accurate.
4. 🚀 Submit a Pull Request (PR) with a clear explanation of the addition.

---

## ⚠️ Disclaimer

- This list is **community-curated** for educational and research purposes — it does not constitute an endorsement.
- Industrial predictive maintenance involves critical asset safety. Evaluate security controls, access models, and safety compliance before deploying self-hosted software in production environments.
- Verify software licenses and organizational maturity prior to commercial adoption.

---

<p align="center">
  <b>Curated with ❤️ for Maintenance Engineers, Reliability Professionals &amp; Industrial AI Researchers</b><br/>
  <i>Awesome-Awesome-Awesome List Collection: <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome">Awesome-Awesome-Awesome</a></i>
</p>
