# Zindi_lightautoml_baseline

This is a repo for [AutoInland Vehicle Insurance Claim Challenge](https://zindi.africa/competitions/autoinland-vehicle-insurance-claim-challenge) baseline based on [LightAutoML](https://github.com/sberbank-ai-lab/LightAutoML).

**Current score is 0.3252**

P.S. We will be happy for your ⭐️ on LightAutoML repo if you like it.

---

## Prerequisites

LightAutoML installation from PyPI:
```
pip install -U lightautoml
```

To make the code more suitable for your computational resources please change the `N_THREADS` for the number of threads to train LightAutoML model on your machine.

---

## The structure of baseline:

- LightAutoML installation
- Parameters setup
- Data loading
- Feature engineering
- Splitting train dataset into training and validation parts
- Train basic model and:
    - check the score on validation part
    - check feature importances
    - optimize the threshold for F1
- Train timeout utilization model and:
    - check the score on validation part
    - check feature importances
    - optimize the threshold for F1
- Select the best model from upper two and retrain it on the full training dataset
- Prepare submission
