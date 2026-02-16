<h1 align="center">metalflare</h1>

<h4 align="center">Computational investigation of a Cu(I)-sensing green fluorescent protein</h4>

<p align="center">
    <a href="https://github.com/durrantlab/metalflare/releases">
        <img src="https://img.shields.io/github/v/release/durrantlab/metalflare" alt="GitHub release (latest by date)">
    </a>
    <a href="https://github.com/durrantlab/metalflare/" target="_blank">
        <img src="https://img.shields.io/github/repo-size/durrantlab/metalflare" alt="GitHub repo size">
    </a>
    <a href="https://doi.org/10.5281/zenodo.15549425"><img src="https://zenodo.org/badge/719581358.svg" alt="DOI"></a>
</p>

Metalflare is a computational study investigating the molecular mechanisms underlying copper(I) sensing by roGFP2, a genetically encoded fluorescent protein.
This work combines molecular dynamics simulations with experimental validation to understand how roGFP2 achieves sub-femtomolar Cu(I) binding affinity and generates robust ratiometric fluorescence changes.

The project explores the structural basis for roGFP2's dual functionality as both a redox sensor and copper probe, revealing distinct spectroscopic signatures and molecular mechanisms for each sensing mode.

## Background

Copper is essential for cellular processes including mitochondrial respiration, antioxidant defense, and neurotransmission, yet excess copper can trigger toxic redox reactions and cell death.
Cells maintain extremely low free copper concentrations, making intracellular copper detection challenging.
While genetically encoded sensors have revolutionized calcium and zinc imaging, copper detection has proven uniquely difficult due to copper's low bioavailability, tight coordination, and redox lability.
This study demonstrates that roGFP2, originally engineered as a redox sensor, can serve as a high-affinity Cu(I) probe with superior performance compared to existing copper sensors.

## Computational Methods

This repository contains all scripts for preparing, running, and analyzing classical molecular dynamics simulations performed on three roGFP2 states.

- **Structures**: Reduced (PDB: 1JC0), oxidized (PDB: 1JC1), and Cu(I)-bound roGFP2.
- **Environment**: Explicit water with 150 mM NaCl.
- **Conditions**: NPT ensemble at 300 K and 1 atm.
- **Duration**: Three independent trajectories of 500 ns each (1.5 μs total per system).
- **Analysis**: Structural dynamics, hydrogen bonding networks, and chromophore conformations.

## Key Computational Findings

Molecular dynamics simulations reveal that Cu(I) coordinates directly between Cys147 and Cys204, causing an expansion of the Cα-Cα distance by approximately 0.44 Å compared to the reduced state.
This metal binding propagates allosteric changes to the chromophore environment, particularly disrupting the critical Gln94-chromophore hydrogen bond that normally stabilizes fluorescence.
The resulting enhanced chromophore flexibility opens non-radiative decay pathways, explaining the selective B-band quenching observed experimentally.

## Getting Started

This project uses [Pixi](https://pixi.prefix.dev/latest/) for reproducible environment management.
You'll need to install Pixi first:

```bash
curl -fsSL https://pixi.sh/install.sh | sh
```

Clone the repository and set up the computational environment:

```bash
git clone git@github.com:durrantlab/metalflare.git
cd metalflare
pixi install --locked
```

This installs Python along with all required dependencies including MDAnalysis, scientific computing libraries, and specialized tools like AmberTools and PyMOL for molecular analysis.

## License

Code contained in this project is released under the [MIT][mit] as specified in [`LICENSE.md`](https://github.com/durrantlab/metalflare/blob/main/LICENSE.md).
All other data, information, documentation, and associated content provided within this project are released under the [CC BY 4.0][cc-by-4.0] as specified in [`LICENSE_INFO.md`](https://github.com/durrantlab/metalflare/blob/main/LICENSE_INFO.md).

[mit]: https://spdx.org/licenses/MIT.html
[cc-by-4.0]: https://creativecommons.org/licenses/by/4.0/
