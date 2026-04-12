# Akintoye Oyedola — Portfolio

Personal portfolio site hosted at [Akintoye06.github.io](https://Akintoye06.github.io), showcasing research and technical work in cybersecurity, wireless network security, IoT systems, and biometric authentication.

## Projects

### 01 · Beacon Frame Analysis for Passive Rogue AP Detection
Passive, client-agnostic detection pipeline analyzing IEEE 802.11 Layer 2 management frames to distinguish legitimate APs from evil-twin rogue devices. Includes supervised ML classifiers (Random Forest, SVM), a rule-based CLI detection script, and qualitative analysis of MAC randomization and SSID cloaking failure modes under RFC 9414.

**Key results:** 83% rogue class recall, AUC 0.80 (Random Forest), 593 labeled management frames across 8 capture sessions.

**Tools:** Python, Scapy, scikit-learn, Kali Linux, airodump-ng, Wireshark

---

### 02 · Measurement Bias in Wearable PPG Sensors
Literature review tracing the causal chain from PPG sensor optical physics (melanin absorption at 660 nm and 940 nm) through AI training pipelines to clinical harm and regulatory failure. Evaluates FDA and EU AI Act frameworks against five identified policy gaps and proposes five targeted recommendations.

**Key findings:** 20% occult hypoxemia error rate in contemporary devices (EquiOx 2025); no binding pre-market standard exists in any jurisdiction despite FDA acknowledgment in 2021.

**Coverage:** 18 sources across IEEE Xplore, PubMed, FDA.gov, EUR-Lex, WHO

---

### 03 · EEG-Based Biometric Authentication at Clinical Scale
Reproducibility study evaluating five published EEG authentication methods on 2,993 clinical recordings from the Temple University Hospital TUABEXB corpus under subject-disjoint 5-fold cross-validation — the first work to quantify the reproducibility gap between small-dataset lab results and clinical-scale evaluation. Companion work built and evaluated a hybrid EEGNet + ResNet18 + CNN-LSTM architecture.

**Key results:** EEGNet baseline 83.46% ± 0.95% accuracy; all five replicated methods show 13–20 percentage point drops vs. originally reported values; per-channel z-score normalization identified as the single most impactful factor.

**Tools:** Python, PyTorch, MNE-Python, scikit-learn, Google Colab (H100 GPU)

---

### 04 · Dynamic Value Asymmetry in Ransomware Negotiation Models
Game-theoretic analysis of the Vakilinia et al. (2021) smart contract-based ransomware negotiation framework. Formalizes two unaddressed modeling gaps — attacker minimum value exceeding the victim Shapley value, and static treatment of a dynamically depreciating victim valuation — and proposes a time-parameterized mechanism with Chainlink Automation integration preserving incentive compatibility for both parties.

**Tools:** Game theory, mechanism design, Solidity (smart contract design), Chainlink Automation

---

## Repo Structure

```
akinoyedola.github.io/
├── index.html           # Portfolio site
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

## Setup

The site is plain HTML and CSS — no build step, no dependencies, no framework. To run locally, open `index.html` directly in a browser. To deploy, enable GitHub Pages in the repository settings and set the source to the root of the `main` branch.

## Contact

[linkedin.com/in/akintoye-oyedola-a82607214](https://linkedin.com/in/akintoye-oyedola-a82607214/)  
akinoyedola@proton.me  
[github.com/Akintoye06](https://github.com/Akintoye06)
