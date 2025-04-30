# RG-NJL-EoS-tables
This repository includes tabulated equations of state for three-flavor quark matter calculated with the Renormalization Group - consisten Nambu Jona-Lasinio (RG-NJL) model CITE. The three equations of state RG-NJL1 (soft), RG-NJL2 (intermediate) and RG-NJL3 (stiff) refer to the equations of state presented in detail in CITE. They can be combined with a hadronic equation of state to construct hybrid equations of state. Publications using the RG-consistent NJL model include [[1]](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.111.014006), [[2]](https://arxiv.org/abs/2411.04064), [[3]](https://arxiv.org/abs/2503.13626).

# Usage and format
The equations of state are tabulated as one-dimensional EoS tables of cold beta-equilibrated matter in the CompOSE format [[4]](https://compose.obspm.fr), [[5]](https://link.springer.com/article/10.1134/S1063779615040061), [[6]](https://journals.aps.org/rmp/abstract/10.1103/RevModPhys.89.015007), [[7]](https://arxiv.org/pdf/2203.03209). They can straightforwardly be be interpolated using the CompOSE code. A special feature of the model compared to models on the CompOSE database is that it includes color-superconducting diquark condensates and a first-order phase transition between the tow-flavor superconducting (2SC) phase at lower densities and the color-flavor locked (CFL) phase at higher densities. The values of the color-superconducting condensates are included in the eos.micro file in columns 11-16. The codes 800060, 801060 and 802060 encode the diquark condensates Delta 1 (down-strange pairing), Delta 2 (up-strange pairing) and Delta 3 (up-down pairing), repsectively, the value of which follow are written in the next column.

# Features
Renormalization group-consistency for low-energy models, including diquark condensates, was outlined in [[8]](https://scipost.org/10.21468/SciPostPhys.6.5.056). In the language of the functional renormalization group, it states that the effective potential in the infrared must not depend on the intial UV scale.
The renormalization group - consistent version of the NJL model allows to avoid cutoff artifacts of the conventional regularization. This is of particular importance for the study of color-superconducting quark matter at neutron star densities, as cutoff artifacts lead to unphysical suppression of the diquark condensates which affects the phase structure at nonzero temperatures [[1]](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.111.014006).
In the non-renormalizable NJL model, RG-consistency is ambiguous in the sense that medium divergences need to be cancelled by counterterms and the form of the latter depends on the renormalization scheme. The equation of states here are calculated in the massless scheme, see [[1]](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.111.014006).

# Limitations

The model includes a local vector interaction. This leads to the sound speed asymptotically approaching the speed of light in the large-density limit. This is inconsistent with perturbative QCD . Thus, the tabulated EoSs should be used until a maximum chemical potential from which they can be extrapolated to the pressure of perturbative QCD in a causal and thermodynamically consistent way. For details, see [[2]](https://arxiv.org/abs/2411.04064).

# Future
We intend to provide two-dimensional (nonzero temperature) and three-fimensional (arbitrary charge fraction) tables for this model with different RG-consistent schemes soon. Furthermore, the underlying code to generate equations of state in the RG-NJL model is going to become publicly available as a part of [MUSES](https://gitlab.com/nsf-muses), so stay tuned.

# References

[1] H. Gholami, M. Hofmann, and M. Buballa, Phys. Rev. D 111, 014006 (2025), arXiv:2408.06704 [hep-ph].  
[2] H. Gholami, I. A. Rather, M. Hofmann, M. Buballa, and J. Schaffner-Bielich, (2024), arXiv:2411.04064 [hep-ph].    
[3] J.-E. Christian, I. A. Rather, H. Gholami and M. Hofmann, (2025), arXiv:2503.13626 [astro-ph.HE].  
[4] https://compose.obspm.fr  
[5] S. Typel, M. Oertel, and T. Klähn, Phys. Part. Nucl. 46, 633 (2015), arXiv:1307.5715 [astro-ph.SR].  
[6] M. Oertel, M. Hempel, T. Klähn, and S. Typel, Rev. Mod. Phys. 89, 015007 (2017).  
[7] S. Typel et al. (CompOSE Core Team), Eur. Phys. J. A 58, 221 (2022), arXiv:2203.03209 [astro-ph.HE].  
[8] J. Braun, M. Leonhardt, and J. M. Pawlowski, SciPost Phys. 6, 056 (2019), arXiv:1806.04432 [hep-ph].  
