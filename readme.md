# Modified Teukolsky Equation for EMRIs in Matter Environments

![EMRI in environment](deformedringwaves.png)

Computational supplementary material for the paper **"Towards relativistic inspirals into black holes surrounded by matter"** by Lukáš Polcar and Vojtěch Witzany (2025), ArXiv: 2507.XXXXX.

## Repository Contents

### Mathematica Notebooks

#### `ModifiedTeukolsky.nb`
Derivation of the modified Teukolsky equation with explicit forms of individual terms.
*Corresponds to Sections II E, II F, and Appendix B*

#### `Sourceincoordinates.nb`
Evaluation of the modified effective source localized on the matter shell in Schwarzschild coordinates. Solves the (1,1) equations for the ring dynamics.
*Corresponds to Section IV*

#### `SourceinNPGHPformalism.nb`
Two-part notebook:
- **Part 1** (A. Spiers): Newman-Penrose and Geroch-Held-Penrose formalism setup, perturbed NP scalar computations
- **Part 2** (L. Polcar): Effective source construction using reconstructed (0,1) metric via Hertz potential, decomposition into spin-weighted spherical harmonics

*Corresponds to Section IV*

#### `Thebackgroundspacetime.nb`
Background spacetime derivation using Israel junction conditions to match linearized Kerr solutions. Computes (1,0) Newman-Penrose quantities and stress-energy tensor on the matter shell.
*Corresponds to Section III and Appendix C*

### Datasets

In addition to the four Mathematica notebooks, this supplemental material includes a collection of dataset files containing precomputed amplitudes of the forcing terms in the perturbed geodesic equation of the ring. These files are used by the notebook Sourceincoordinates.nb to avoid recomputation during evaluation.

Each dataset file is named according to the orbital parameters of the point particle and the radius 
𝑟
r of the ring, using the format:

php-template
Zkopírovat
Upravit
i<inclination>_p<semilatus rectum>_e<eccentricity>_r<radius>.dat
For example, the file i0.5_p12.0_e0_r20.0.dat corresponds to a particle orbit with inclination 0.5, semilatus rectum 12.0, eccentricity 0, and ring radius 20.0.

Each line in the file contains the following data:

Mode numbers 
𝑚
m, 
𝑛
n, and 
𝑘
k

The corresponding mode frequency

The complex amplitudes of the four components of the source in the perturbed geodesic equation, given in the order: real part and imaginary part of each amplitude

## Citation

Please lookup the citation key on InspireHEP for bibliographic updates

```bibtex
@article{Polcar:2022XXX,
    author = "Polcar, Luk{\'a}{\v{s}} and and Witzany, Vojt{\v{e}}ch",
    title = "{Towards relativistic inspirals into black holes surrounded by matter}",
    eprint = "2507.XXXXX",
    archivePrefix = "arXiv",
    primaryClass = "gr-qc",
    journal = "Submitted to Phys. Rev. D",
    year = "2025"
}

```

For NP/GHP formalism components, also cite:
- A. Spiers, A. Pound, and J. Moxon, Phys. Rev. D **108**, 064002 (2023)

## Authors

- Lukáš Polcar
- Vojtěch Witzany  
