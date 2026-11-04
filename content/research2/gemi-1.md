# Prof. Yi Wang (王艺) | Academic Homepage & Research Laboratory

> **Professor**, School of Computer Science and Technology, Dongguan University of Technology  
> **Email:** wangyi@dgut.edu.cn  
> **Research Focus:** Pattern Recognition, Machine Learning, Adversarial Machine Learning, Federated Learning, and Generative Data Augmentation[cite: 1, 3]

---

## 💡 Research Overview

Modern deep learning systems serve as critical infrastructure across computer vision, biometric security, medical imaging, and collaborative computing[cite: 21, 26]. However, deep learning models remain vulnerable to adversarial attacks, privacy leakage, and data distribution shifts[cite: 5, 7, 10, 26]. 

Our research laboratory focuses on **Pattern Recognition and Machine Learning**[cite: 3], bridging **Adversarial Machine Learning (AML)**[cite: 4, 26] and **Generative Data Augmentation**[cite: 17, 19, 24]. By understanding model vulnerabilities through perturbation design, we build secure, robust, privacy-preserving, and computationally efficient machine learning models[cite: 3, 24, 26].

---

## 🎯 Research Interests & Primary Deliverables

                     [ Research Scope ]
                             │
 ┌───────────────────────────┼───────────────────────────┐                           

1. Adversarial ML           2. Collaborative Training     3. Generative Models

* Attack & Defense          - Federated Learning          - Data Distillation
* Detection & Robustness    - Knowledge Distillation      - PEFT & Synthesis


---

### 1. Adversarial Machine Learning: Attack, Defense & Robustness

Adversarial machine learning investigates the trade-off between model utility and security under open-world, static, and dynamic threats[cite: 4, 5, 26].

* **Query-Efficient Adversarial Attacks:**
  * Developed **DAIR**, a query-efficient decision-based black-box attack tailored for Content-Based Image Retrieval (CBIR) systems[cite: 4, 6]. DAIR reduced system query overhead by **87%** while successfully bypassing commercial visual search engines such as Microsoft Bing[cite: 6].
  * Studied smart adversarial attacks on deep hashing-based retrieval and tree ensemble classifiers[cite: 4].
* **Model-Agnostic Adversarial Detection:**
  * Proposed detection mechanisms by applying random perturbations to input space and leveraging output statistical change patterns to catch low-magnitude adversarial noise[cite: 4, 26].
* **Ensemble & Feature Robustness Enhancement:**
  * **Priority Diversified Dropout (PDD)** & **Dispersed Ensemble Gradients (DEG):** Introduced multi-view base-network feature diversification to optimize ensemble model robustness against gradient-based attacks[cite: 8].
  * Disentanglement of deep features for face detection adversarial robustness[cite: 4].

---

### 2. Collaborative Training, Federated Learning & Knowledge Distillation

Collaborative computing faces severe challenges under non-IID (long-tailed) data distributions, client heterogeneity, privacy leakage, and communication bottlenecks[cite: 7, 10, 22].

* **Federated Learning under Long-Tailed Heterogeneity:**
  * **FedHyb / FedDDL Framework:** Combined instance-based sampling at the client side with class-balanced proxy dataset ensemble distillation at the server side, resolving classifier bias and smoothing loss landscapes under extreme non-IID settings ($\alpha=0.5$, $IF=100$)[cite: 10, 12, 13].
* **Adaptive Adversarial Distillation (AdaAD):**
  * Optimized small-capacity student model training within an adversarial game framework by dynamically searching alignment anchor points, improving both standard accuracy and adversarial robustness[cite: 14].
* **Privacy Inference & Leakage Auditing:**
  * Demonstrated individual property inference, sample reconstruction, and membership inference vulnerabilities in deep feature spaces during collaborative model updates[cite: 7, 9].
* **One-Shot Federated Learning:**
  * **SEDAG Framework:** Achieved single-round server aggregation via data-free multi-expert distillation, cutting client-side communication costs and exposure to poisoning threats[cite: 22].

---

### 3. Generative Data Augmentation, Data Distillation & Model Tuning

Generative models (GANs, Diffusion Models, and Auto-regressive Transformers) provide structured, domain-constrained perturbations that solve data scarcity, domain shifts, and privacy constraints[cite: 16, 24].

* **Robustness Feature Adapter (RFA):**
  * Plug-and-play adapter inserted into backbone feature spaces (e.g., Vision Transformers). RFA generates dynamic adversarial perturbations during training, accelerating ViT adversarial training by **>4×** while cutting parameter overhead to **<1/10** and yielding **>50%** robustness gains[cite: 17, 18].
* **Influence-Guided Diffusion (IGD) for Dataset Distillation:**
  * Introduced target-gradient guidance during reverse diffusion sampling, enabling training-free, task-adaptive proxy dataset generation for downstream classification tasks (e.g., ResNet, MobileNet, EfficientNet)[cite: 19].
* **Data Likelihood Estimation via Diffusion Reconstruction:**
  * Proposed core-set selection criteria measuring DDPM partial-reconstruction deviations to extract representative sample subsets for incremental learning and edge deployment[cite: 20].
* **Cross-Modal Medical Image Fusion:**
  * **FedMCA:** Cross-attention personalized multimodal federated learning for modality-heterogeneous MRI (T1, FLAIR) segmentation and classification[cite: 21].
* **Physics-Informed Metamaterial Inverse Design:**
  * 3D Conditional Diffusion Models combined with topological derivative data augmentation to synthesize voxelized metamaterial geometry structures with specified elastic modulus and conductivity[cite: 23].

---

## 📑 Selected Publications & Patents

### Representative Publications

| Year     | Title                                                                                                              | Venue / Journal                    | Key Topic                                           |
| :------- | :----------------------------------------------------------------------------------------------------------------- | :--------------------------------- | :-------------------------------------------------- |
| **2026** | *Diffusion Reconstruction-Based Data Likelihood Estimation for Core-Set Selection*[cite: 9, 20]                    | **AAAI 2026**[cite: 20]            | Data Distillation / Diffusion[cite: 20]             |
| **2026** | *FedMCA: Cross-Attention-Based Personalized Multimodal Federated Learning Under Modality Heterogeneity*[cite: 21]  | **ICMSSP 2026**[cite: 21]          | Multimodal Medical FL[cite: 21]                     |
| **2025** | *Robustness Feature Adapter for Efficient Adversarial Training*[cite: 4, 15, 17]                                   | **ECAI 2025**[cite: 17]            | Efficient Adversarial Training / PEFT[cite: 15, 17] |
| **2025** | *Influence-Guided Diffusion for Dataset Distillation*[cite: 9, 15, 19]                                             | **ICLR 2025**[cite: 19]            | Generative Dataset Distillation[cite: 19]           |
| **2025** | *StableGuard: Towards Unified Copyright Protection and Tamper Localisation*[cite: 15]                              | **NeurIPS 2025**[cite: 15]         | AI Safety & Watermarking[cite: 15]                  |
| **2025** | *Optimizing Metamaterial Inverse Design with 3D Conditional Diffusion Model and Data Augmentation*[cite: 23]       | **Adv. Materials Tech.**[cite: 23] | Generative Models in AI for Science[cite: 23]       |
| **2024** | *Federated Learning with Hybrid Knowledge Distillations on Long-Tailed Heterogeneous Client Data*[cite: 9, 12, 13] | **ECAI 2024**[cite: 12, 13]        | Long-Tailed Federated Learning[cite: 12, 13]        |
| **2023** | *Boosting Accuracy and Robustness of Student Models via Adaptive Adversarial Distillation*[cite: 4, 9, 14]         | **IEEE/CVF CVPR 2023**[cite: 14]   | Adversarial Knowledge Distillation[cite: 14]        |
| **2022** | *Individual Property Inference Over Collaborative Learning In Deep Feature Space*[cite: 7, 9]                      | **IEEE ICME 2022**[cite: 7]        | Privacy Leakage in FL[cite: 7]                      |
| **2021** | *DAIR: A Query-Efficient Decision-Based Attack On Image Retrieval Systems*[cite: 4, 6]                             | **ACM SIGIR 2021**[cite: 6]        | Black-Box CBIR Attack[cite: 6]                      |
| **2021** | *Adversarial Defence By Diversified Simultaneous Training Of Deep Ensembles*[cite: 4, 8]                           | **AAAI 2021**[cite: 8]             | Deep Ensemble Robustness[cite: 8]                   |

### Key Grants & Intellectual Property
* **National Natural Science Foundation of China (NSFC) General Program:** *Research on Privacy and Security Issues in Biometric Recognition and Retrieval under Adversarial Environments* (Grant No. 61876040, Direct Cost: 650,000 RMB)[cite: 4].
* **Guangdong Basic and Applied Basic Research Foundation Joint Grant:** *Smart Processing of Vital Sign Signals at the Edge* (Co-PI with Sun Yat-sen University)[cite: 9].
* **Patents:** Holder of multiple US and Chinese National Invention Patents regarding adversarial detection, secure hashing retrieval, and privacy-preserving federated training[cite: 4, 9].

---

## 👤 Biography & Career Path

Prof. Yi Wang received her academic training across top international institutions in Australia, Hong Kong, and Mainland China[cite: 2].




2002–2009       2009–2012             2012–2017                   2017–Present
Univ. of        UNSW Sydney           Hong Kong Baptist Univ.     Dongguan Univ. of Tech.
Melbourne       Postdoc / Res. Assoc. Research Assistant Prof.    Full Professor
(Researcher)    (Math & CS)           (Computer Science)          (Computer CS Dept.)


* **2017 – Present:** Full Professor, School of Computer Science and Technology, Dongguan University of Technology (National High-Level Overseas Talent)[cite: 2].
* **2012 – 2017:** Research Assistant Professor / Research Associate, Department of Computer Science & Institute of Computational and Theoretical Studies, Hong Kong Baptist University[cite: 2].
* **2009 – 2012:** Postdoctoral Fellow / Research Associate, School of Mathematics and Statistics & CSE, University of New South Wales (UNSW Sydney)[cite: 2].
* **2003 – 2004:** Research Assistant, University of Melbourne & City University of Hong Kong[cite: 2].

---

## 📬 Contact & Graduate Student Admissions

Our laboratory welcomes self-motivated Master’s students, PhD candidates, and Postdoctoral Researchers interested in **Pattern Recognition, Adversarial Safety, Generative AI, and Federated Learning**[cite: 1, 3, 25].

* **Office:** School of Computer Science and Technology, Dongguan University of Technology, Songshan Lake Campus, Dongguan, Guangdong, China[cite: 1, 4]
* **Email:** [wangyi@dgut.edu.cn](mailto:wangyi@dgut.edu.cn)[cite: 4, 25]
* **WeChat Contact:** Wang Yi (Alice)[cite: 25]

