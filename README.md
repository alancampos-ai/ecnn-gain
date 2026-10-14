# Ecnn gain 

#### Article:   <small><strong>Equivariant switching-isomorphism for gain dipoles</strong>  <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>  <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>  <a href="https://drive.google.com/drive/folders/1BTz5JVhngoo7FBVmnOYBjNtRcnw5g8UJ?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We enumerate switching-isomorphism classes of gain assignments on the $m$-edge dipole $D_m$ over any finite group $G$. An equivariant multiset quotient gives an exact cycle-profile Burnside algorithm avoiding enumeration of $G^m$ and $S_m$. For $n=|G|$ and $R$ retained cycle profiles, it uses $O(n^3+Rnm^2)$ arithmetic operations and $O(n^2+Rn+m)$ stored integer entries. For finite abelian groups, prime-power counts recover the primary structure when $|G|$ is known, while the complete count sequence determines $|G|$. The study covers $31$ configurations, $20$ seeds, and $6{,}820$ executions across eleven methods. Cycle-profile enumeration completes all $620$ cases, and every completed method returns the same count. In $19$ fully paired configurations, median runtime reductions are $99.08\%$ against Direct Burnside and $45.18\%$ against Cyclewise theorem. Holm-adjusted Wilcoxon tests favor Cycle-profile enumeration in $19/19$ and $14/19$ configurations, respectively. Six methods incur $540$ timeouts in the extended settings. Each execution uses two untimed warm-ups and five to fifteen measured repetitions, retaining the median wall time. Multiset generator orbit is faster in the primary comparison, with a median compared-time/profile-time ratio of $0.851$.

#### Dependencies

* Python 3.10.19
* NumPy 1.26.4
* Matplotlib 3.10.8

#### Installation

```bash
docker build -f docker/Dockerfile -t gain-dipole-equivalence:main .
docker run --rm --cpus=1 --memory=2g -v "$(pwd)/results:/workspace/results" gain-dipole-equivalence:main
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
