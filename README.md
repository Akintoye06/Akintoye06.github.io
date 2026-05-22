# Akintoye Oyedola — Portfolio

Personal portfolio site hosted at [akintoye06.github.io](https://akintoye06.github.io/), showcasing research and technical work in cybersecurity, HPC systems administration, wireless network security, IoT systems, and biometric authentication.

---

## Projects

### 01 · HPC Cluster Administration at UNF

End-to-end deployment and administration of a KVM-based OpenHPC cluster at the University of North Florida — from bare-metal provisioning through Open OnDemand portal deployment and GPU metrics collection. Covers Rocky Linux 9.7 cluster build, Slurm/Munge configuration, NFS infrastructure, systemd service management, and a Telegraf-based GPU monitoring pipeline using NVIDIA tooling.

**Repos:** [openhpc](https://github.com/Akintoye06/openhpc) · [open-ondemand](https://github.com/Akintoye06/open-ondemand) · [gpu-monitoring](https://github.com/Akintoye06/gpu-monitoring)  
**Tools:** OpenHPC, Slurm, Munge, KVM, NFS, Open OnDemand, Telegraf, NVIDIA, Rocky Linux 9.7, systemd

---

### 02 · Benchmarking EEG-Based Authentication at Clinical Scale: A Reproducibility Study

Two-dataset reproducibility study evaluating five published deep learning EEG authentication methods on 2,993 clinical recordings from the Temple University Hospital TUABEXB corpus, and replicating Wang et al.'s DE-CNN on the original SEED dataset under subject-disjoint evaluation. Decomposes the reproducibility gap into a 59.77pp protocol effect and a 16.24pp dataset scale effect — the first work to isolate these two contributors at clinical scale. Submitted to Biomedical Signal Processing and Control (Elsevier).

**Key results:** EEGNet baseline 83.46% ± 0.95% on TUABEXB; all five replicated methods show 13–20pp accuracy drops vs. originally reported values; Wang et al.'s 99.7% on SEED collapses to 39.93% under subject-disjoint evaluation, revealing a 59.77pp protocol effect; per-channel z-score normalization identified as the single most impactful factor.  
**Tools:** Python, PyTorch, MNE-Python, scikit-learn, Google Colab (H100 GPU)  
**Code:** [eeg-authentication-reproducibility](https://github.com/Akintoye06/eeg-authentication-reproducibility)

---

### 03 · Beacon Frame Analysis for Passive Rogue AP Detection

Passive, client-agnostic detection pipeline analyzing IEEE 802.11 Layer 2 management frames to distinguish legitimate APs from evil-twin rogue devices. Includes supervised ML classifiers (Random Forest, SVM), a rule-based CLI detection script, and qualitative analysis of MAC randomization and SSID cloaking failure modes under RFC 9414.

**Key results:** 83% rogue class recall, AUC 0.80 (Random Forest), 593 labeled management frames across 8 capture sessions.  
**Tools:** Python, Scapy, scikit-learn, Kali Linux, airodump-ng, Wireshark

---

### 04 · Measurement Bias in Wearable PPG Sensors

Literature review tracing the causal chain from PPG sensor optical physics (melanin absorption at 660 nm and 940 nm) through AI training pipelines to clinical harm and regulatory failure. Evaluates FDA and EU AI Act frameworks against five identified policy gaps and proposes five targeted recommendations.

**Key findings:** 20% occult hypoxemia error rate in contemporary devices (EquiOx 2025); no binding pre-market standard exists in any jurisdiction despite FDA acknowledgment in 2021.  
**Coverage:** 18 sources across IEEE Xplore, PubMed, FDA.gov, EUR-Lex, WHO

---

### 05 · Dynamic Value Asymmetry in Ransomware Negotiation Models

Game-theoretic analysis of the Vakilinia et al. (2021) smart contract-based ransomware negotiation framework. Formalizes two unaddressed modeling gaps — attacker minimum value exceeding the victim Shapley value, and static treatment of a dynamically depreciating victim valuation — and proposes a time-parameterized mechanism with Chainlink Automation integration preserving incentive compatibility for both parties.

**Tools:** Game theory, mechanism design, Solidity (smart contract design), Chainlink Automation

---

## Repo Structure

```
Akintoye06.github.io/
├── index.html           # Portfolio site
├── resume.pdf           # Downloadable resume
├── Akintoye_Headshot.jpeg
├── papers/
│   ├── rogue-ap-conference.pdf
│   ├── rogue-ap-report.pdf
│   ├── rogue-ap-poster.pdf
│   ├── ppg-bias-conference.pdf
│   ├── ppg-bias-report.pdf
│   ├── ppg-bias-poster.pdf
│   ├── eeg-benchmarking.pdf
│   ├── eeg-cnn-poster.pdf
│   └── ransomware-negotiation.pdf
└── README.md
```

---

## Setup

The site is plain HTML and CSS — no build step, no dependencies, no framework. To run locally, open `index.html` directly in a browser. To deploy, enable GitHub Pages in the repository settings and set the source to the root of the `main` branch.

---

## Contact

- LinkedIn: [linkedin.com/in/akintoye-oyedola-a82607214](https://www.linkedin.com/in/akintoye-oyedola-a82607214/)
- Email: [akinoyedola@proton.me](mailto:akinoyedola@proton.me)
- GitHub: [github.com/Akintoye06](https://github.com/Akintoye06)
