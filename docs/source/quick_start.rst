Quick Start
==============


HyperBox是工具包, 帮助用户设计神经网络架构搜索算法，是一款轻量级库，易于使用，便于扩展。

### HyperBox核心支持

- Pytorch Lightning

Why PyTorch Lightning?
PyTorch Lightning is a lightweight PyTorch wrapper for high-performance AI research. It makes your code neatly organized and provides lots of useful features, like ability to run model on CPU, GPU, multi-GPU cluster and TPU.

- Hydra

Why Hydra?
Hydra is an open-source Python framework that simplifies the development of research and other complex applications. The key feature is the ability to dynamically create a hierarchical configuration by composition and override it through config files and the command line. It allows you to conveniently manage experiments and provides many useful plugins, like Optuna Sweeper for hyperparameter search, or Ray Launcher for running jobs on a cluster.


### HyperBox重要概念

- Mutable 所有可变对象
  - Space 
    - CategoricalSpace 离散的空间
    - OperationSpace 候选操作组成的离散空间
    - InputSpace 可选的输入空间，从其中挑选某个作为输入
    - ValueSpace 更加细粒度的搜索空间，可以控制内部属性，比如Conv中的kernel,channel等属性。
  - Op 所有候选操作
- Mutator 主动改变Mutable对象或者其内部属性