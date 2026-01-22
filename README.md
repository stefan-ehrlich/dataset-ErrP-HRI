# dataset-ErrP-HRI

**Dataset: A feasibility study for validating robot actions using EEG-based error-related potentials (ErrP)**

This repository contains the dataset accompanying the publication:

> **Ehrlich, S. K., & Cheng, G. (2019).**  
> *A feasibility study for validating robot actions using EEG-based error-related potentials.*  
> **International Journal of Social Robotics, 11(2), 271–283.**  
> http://dx.doi.org/10.1007/s12369-018-0501-8

The dataset is designed for research on **error-related potentials (ErrP)** in **human–robot interaction (HRI)**, where ErrPs are elicited when a human observes robot behavior that is **incorrect** or **unexpected**.

---

## Repository structure

```text
dataset-ErrP-HRI/
├── cursor/                              # EEG data: "cursor" condition / scenario
│   └── s01
│   └── s02
│   └── ...
├── robot/                               # EEG data: "robot" condition / scenario
│   └── s01
│   └── s02
│   └── ...
├── documentation_dataset-ErrP-HRI.pdf    # dataset documentation (recommended)
└── README.md
```

## Study description (brief)

### ErrP dataset in HRI observation tasks
**Purpose:** provide EEG recordings that allow analysis and classification of **error-related potentials (ErrP)** elicited by **observed robot actions**.

**Design:** Participants observed system behavior across different scenarios/conditions. Trials are annotated such that EEG epochs can be assigned to **error vs. correct** events (and potentially further task phases depending on the dataset documentation).

This dataset supports typical ErrP pipelines such as:
- epoch extraction around **error/non-error** events
- ERP averaging and statistical analysis
- single-trial classification (e.g., **LDA / SVM / Riemannian / CNN** baselines)

---

## About the dataset

### Intended use
This dataset supports research in:
- ErrP detection and modeling
- passive BCI for **human–robot interaction**
- neuroergonomics (**implicit feedback signals**)
- evaluation of robust EEG classification under realistic HRI conditions

### Modalities and measures (overview)
Depending on the condition folder (`cursor/`, `robot/`), the dataset includes:
- **EEG recordings**
- **event markers / labels** enabling error vs. correct segmentation
- scenario-dependent task metadata

For exact data formats, EEG configuration, event codes, and label semantics, consult the provided documentation.
- `documentation_dataset-ErrP-HRI.pdf`

---

## Citation
If you use this data please cite below publication.

```bibtex
@article{ehrlich2019feasibility,
  title   = {A feasibility study for validating robot actions using eeg-based error-related potentials},
  author  = {Ehrlich, Stefan K. and Cheng, Gordon},
  journal = {International Journal of Social Robotics},
  volume  = {11},
  number  = {2},
  pages   = {271--283},
  year    = {2019},
  doi     = {10.1007/s12369-018-0501-8}
}
