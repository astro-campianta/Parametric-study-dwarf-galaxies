# Parametric-study-dwarf-galaxies

This repository contains Python codes developed as part of my PhD research, based on the work presented in:

C. Pianta, R. Capuzzo-Dolcetta, G. Carraro (2022)
The Impact of Binaries on the Dynamical Mass Estimate of Dwarf Galaxies,
The Astrophysical Journal, 939:3.
[https://doi.org/10.3847/1538-4357/ac9303](https://doi.org/10.3847/1538-4357/ac9303)

---

## Overview

Binary stars are known to affect the dynamical evolution of stellar systems and can inflate the observed velocity dispersion of dwarf spheroidal (dSph) and ultra-faint dwarf (UFD) galaxies. This, in turn, may lead to a significant overestimation of their dynamical masses, with important implications for dark matter studies.

The codes provided here implement parametric models of dSph and UFD galaxies, focusing on the role of unresolved binary stars. For simplicity, only the random pairing method for binary mass assignment is included (the alternative q-distribution method is not implemented in this version). Each code block is preceded by a theoretical explanation, including the relevant formulas, to clarify its purpose and scientific background.

---

## Features

The repository includes Python scripts to:

* generate parametric models of dwarf galaxies;
* build binary populations using the random pairing method, both with and without RLOF rejection;
* read and fit isochrones to extrapolate mass and luminosity values for MS and RGB stars;
* compute the dynamical mass of model galaxies using velocity dispersion, including the contribution of unresolved binaries;
* perform linear interpolation of the velocity dispersion to estimate the dynamical mass;
* calculate the half-mass relaxation time;
* evaluate the relative mass overestimation (ΔM/M) caused by binaries;
* estimate the mass-to-light ratio (M/L) in the U, V, and B photometric bands;
* produce graphical outputs illustrating the effects of different binary fractions and orbital parameter distributions on the velocity dispersion and the dynamical mass.

---

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/dwarf-galaxy-binaries.git
   cd dwarf-galaxy-binaries
   ```

2. Run the Python scripts (examples provided in the `examples/` folder).
   Each script includes comments explaining input parameters and outputs.

3. Generated plots will show:

   * velocity dispersion as a function of binary parameters;
   * dynamical mass estimates with and without binary contamination;
   * relative mass overestimation (ΔM/M) for different binary fractions;
   * mass-to-light ratio (M/L) in U, V, and B bands.

---

## Scientific Context

These tools reproduce the methodology and results presented in Pianta et al. (2022), where we showed that:

* the inflation of the observed velocity dispersion is most sensitive to the semimajor axis distribution of binaries;
* even a small fraction of unresolved binaries can cause a significant overestimate of the dynamical mass in ultra-faint dwarf galaxies;
* this effect is less prominent, but still present, in classical dSph galaxies.

Thus, binaries represent a non-negligible systematic effect in interpreting the kinematics of faint stellar systems.

---

## Citation

If you use these codes in your research, please cite:

```
@article{Pianta2022,
  author = {Pianta, C. and Capuzzo-Dolcetta, R. and Carraro, G.},
  title = {The Impact of Binaries on the Dynamical Mass Estimate of Dwarf Galaxies},
  journal = {The Astrophysical Journal},
  volume = {939},
  number = {3},
  year = {2022},
  doi = {10.3847/1538-4357/ac9303}
}
```

---

## License

This project is released under the MIT License. See `LICENSE` for details.



