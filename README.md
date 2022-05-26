# Differentially Private Covariance Revisited
This repo contains code for implementations of the algorithms and experiments in the paper "Differentially Private Covariance Revisited".

| Folder name     | Description                                                                                                |
| ----------------| ---------------------------------------------------------------------------------------------------------- |
| adaptive        | implementations for our algorithms and the Gaussian mechanism                                              |
| exponential     | implementation for EMCov (exponential mechanism)                                                           |
| coinpress       | a copy of the code from https://github.com/twistedcubic/coin-press, containing implementation of coinpress |


## Requirements
The algorithms and experiments were implemented in Python (v3.9).

The following packages are required:

pytorch v1.9.0
scipy 1.8.0
scikit-learn 1.0.1

```setup
conda install pytorch==1.9.0 torchvision==0.10.0 torchaudio==0.9.0 cpuonly -c pytorch
conda install scipy==1.8.0
conda install scikit-learn==1.0.1
```


## Evaluation
To reproduce the results in a specific figure, run its corresponding script listed below.
| File name          | Corresponding figure | Description                                           |
| ------------------ |--------------------- | ----------------------------------------------------- |
| test_d_N1.py       | Figure 1.            | Synthetic dataset test, fixing tr=1         |
| test_Ns.py         | Figure 2(a).            | Synthetic dataset test, various tr        |
| test_d.py          | Figure 2(b).            | Synthetic dataset test, various d       |
| test_n.py          | Figure 2(c).            | Synthetic dataset test, various n      |
| test_rho.py        | Figure 2(d).            | Synthetic dataset test, various rho       |
| test_mnist_fix_n.py  | Figure 3.            | MNIST dataset test        |
| test_news_rho_l2.py  | Figure 4(a)-(c).            | News dataset test, unit l2 norm        |
| test_news_rho_maxl2.py  | Figure 4(d)-(e).            | News dataset test, normalized by max l2 norm       |

For example, to run the test in Figure 1:
```test
python test_d_N1.py
```



