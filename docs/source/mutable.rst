##########################
可变模块
##########################


整体架构：

```

├── configs                 <- Hydra configuration files
│   ├── callbacks               <- Callbacks configs
│   ├── datamodule              <- Datamodule configs
│   ├── experiment              <- Experiment configs
│   ├── hparams_search          <- Hyperparameter search configs
│   ├── hydra                   <- Hydra related configs
│   ├── logger                  <- Logger configs
│   ├── model                   <- Model configs
│   ├── trainer                 <- Trainer configs
│   │
│   └── config.yaml             <- Main project configuration file
│
├── data                    <- Project data
│
├── logs                    <- Logs generated by Hydra and PyTorch Lightning loggers
│
├── notebooks               <- Jupyter notebooks. Naming convention is a number (for ordering),
│                              the creator's initials, and a short `-` delimited description, e.g.
│                              `1.0-jqp-initial-data-exploration.ipynb`.
│
├── tests                   <- Tests of any kind
│   ├── smoke
│   └── unit
│
├── src
│   ├── callbacks               <- Lightning callbacks
│   ├── datamodules             <- Lightning datamodules
│   ├── models                  <- Lightning models
│   ├── utils                   <- Utility scripts
│   │
│   └── train.py                <- Training pipeline
│
├── run.py                  <- Run any pipeline with chosen experiment configuration
│
├── .env.example            <- Template of the file for storing private environment variables
├── .gitignore              <- List of files/folders ignored by git
├── .pre-commit-config.yaml <- Configuration of automatic code formatting
├── conda_env_gpu.yaml      <- File for installing conda environment
├── Dockerfile              <- File for building docker container
├── requirements.txt        <- File for installing python dependencies
├── setup.cgf               <- Configurations of linters and pytest
├── LICENSE
└── README.md

```


..  toctree::
    :maxdepth: 2

    可变模块 <mutables/intro>
    OperationSpace <mutables/operation_space>
    InputSpace <mutables/input_space>
    ValueSpace <mutables/value_space>