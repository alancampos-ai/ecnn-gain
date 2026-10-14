## ecnn-gain

#### Article:   <small><strong>k-clustering</strong>  <a href="https://doi.org/10.1016/j.cam.2026.117584"><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>  <a href="https://doi.org/10.1016/j.cam.2026.117584"><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>  <a href="https://drive.google.com/drive/folders/1YBVxdJ12ujfiddyKyu-Z6pwpmwWGmsDr?usp=drive_link"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

Experiments on DT-MRI datasets evaluate computational feasibility and provide a controlled comparison among Euclidean, Frobenius, Log-Euclidean, and affine-invariant Riemannian formulations. The implementation supports the EUC (`no_spd`), FR (`spd_fr`), LOG (`spd_le`), and AIRM (`airm`) variants, together with Gaussian mixture model (GMM) experiments. The experimental scripts use three classes and implement cross-validation over configurable data subsets. The supplied configurations include 20 data instances, five folds, and multiple random seeds. Clustering quality is assessed using IoU, Dice, Precision, Recall, Accuracy, foreground macro-F1, and global micro-F1. The implementation also records execution time, iteration count, K-means objective values, and GMM log-likelihood values. The experiments compare the computational behavior and clustering results of the four formulations, enabling a quantitative analysis of accuracy and computational cost.

#### Dependencies

* Python >= 3.8
* numpy
* scipy
* dipy
* matplotlib
* pymanopt
* torch (optional; required for CUDA execution)

#### Bash

```bash
pip install numpy scipy dipy matplotlib pymanopt
pip install torch
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
