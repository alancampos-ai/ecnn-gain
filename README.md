## k-clustering

#### Article:   <small><strong>k-clustering</strong>  <a href="https://doi.org/10.1016/j.cam.2026.117584"><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>  <a href="https://doi.org/10.1016/j.cam.2026.117584"><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>  <a href="https://drive.google.com/drive/folders/1YBVxdJ12ujfiddyKyu-Z6pwpmwWGmsDr?usp=drive_link"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We present a generalized *k*–L<sup>α</sup> centroids algorithm for DT-MRI segmentation. The method encompasses classical *k*-means and related variants in Euclidean and Riemannian geometries by representing cluster prototypes as L<sup>α</sup>-centroids. In DT-MRI data, each voxel is represented by a symmetric positive definite (SPD) matrix. Full three-dimensional data are typically represented by 3×3 SPD tensors, whereas 2×2 SPD matrices occur only in reduced two-dimensional settings. All experiments in this work use 3×3 SPD matrices. The SPD cone is an open, convex subset of the space of symmetric matrices and forms a Hadamard manifold under the affine-invariant metric. Within this geometry, weighted centroids are well-defined and unique. Experiments on real DT-MRI volumes assess computational feasibility and provide a direct, controlled comparison between the Euclidean and Riemannian formulations. The accompanying implementation supports the EUC (`no_spd`), FR (`spd_fr`), LOG (`spd_le`), and AIRM (`airm`) formulations, together with *k*–L<sup>α</sup> centroids and Gaussian mixture model (GMM) experiments. The experimental scripts are configured for three classes and support subject-wise cross-validation over configurable subject sets. The supplied experiments use 20 subjects, five folds, and multiple random seeds. Segmentation performance is evaluated using IoU, Dice, Precision, Recall, Accuracy, foreground-macro F1, and global micro F1. The implementation also records execution time, iteration count, clustering objective values, and GMM log-likelihood values. We compare the EUC, LOG, and AIRM formulations and characterize the relationship between performance and computational cost without claiming general superiority for any formulation.

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
```

For CUDA execution:

```bash
pip install torch
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
