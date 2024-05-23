---
# The Repository is ARCHIVED!
### it is now maintained in https://github.com/MicroStep-MIS/thunderstorm-nowcast-microstep <br>(mirrored to https://github.com/ai4os-hub/thunderstorm-nowcast-microstep)
---

UC-MicroStep-MIS-ai4eosc_thunder_nowcast_ml
==============================

[![Build Status](https://jenkins.indigo-datacloud.eu/buildStatus/icon?job=Pipeline-as-code/DEEP-OC-org/UC-MicroStep-MIS-ai4eosc_thunder_nowcast_ml/master)](https://jenkins.indigo-datacloud.eu/job/Pipeline-as-code/job/DEEP-OC-org/job/UC-MicroStep-MIS-ai4eosc_thunder_nowcast_ml/job/master)

Thunderstorm nowcast based on radar data (for agrometeorology)

To launch it, first install the package then run [deepaas](https://github.com/indigo-dc/DEEPaaS):
```bash
git clone https://github.com/MicroStep-MIS/UC-MicroStep-MIS-ai4eosc_thunder_nowcast_ml
cd ai4eosc_thunder_nowcast_ml
pip install -e .
deepaas-run --listen-ip 0.0.0.0
```
The associated Docker container for this module can be found in https://github.com/MicroStep-MIS/UC-MicroStep-MIS-DEEP-OC-ai4eosc_thunder_nowcast_ml.

## Project structure
```
├── LICENSE
├── README.md              <- The top-level README for developers using this project.
├── data
│   └── raw                <- The original, immutable data dump.
│
├── docs                   <- A default Sphinx project; see sphinx-doc.org for details
│
├── models                 <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks              <- Jupyter notebooks. Naming convention is a number (for ordering),
│                             the creator's initials (if many user development), 
│                             and a short `_` delimited description, e.g.
│                             `1.0-jqp-initial_data_exploration.ipynb`.
│
├── references             <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports                <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures            <- Generated graphics and figures to be used in reporting
│
├── requirements.txt       <- The requirements file for reproducing the analysis environment, e.g.
│                             generated with `pip freeze > requirements.txt`
├── test-requirements.txt  <- The requirements file for the test environment
│
├── setup.py               <- makes project pip installable (pip install -e .) so ai4eosc_thunder_nowcast_ml can be imported
├── ai4eosc_thunder_nowcast_ml    <- Source code for use in this project.
│   ├── __init__.py        <- Makes ai4eosc_thunder_nowcast_ml a Python module
│   │
│   ├── dataset            <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features           <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models             <- Scripts to train models and make predictions
│   │   └── api.py         <- Main script for the integration with DEEP API
│   │
│   ├── tests              <- Scripts to perfrom code testing
│   │
│   └── visualization      <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini                <- tox file with settings for running tox; see tox.testrun.org
```
