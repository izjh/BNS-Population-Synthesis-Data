# BNS Population Synthesis Data

This repository contains public data products for the **Fiducial** model of our binary neutron star (BNS) population-synthesis study.

The data files will be provided in HDF5 (`.h5`) format.

## Repository structure

```text
BNS-Population-Synthesis-Data/
├── ZAMS_BNS/
│   ├── z0/
│   ├── z0.2/
│   ├── z0.4/
│   ├── z0.6/
│   ├── z0.8/
│   ├── z1/
│   ├── z1.3/
│   ├── z1.8/
│   └── z2.3/
├── Cosmergers/
└── SKA/
    ├── AA4/
    └── AAstar/
```

## 1. Metallicity-dependent BNS populations

The `ZAMS_BNS/` directory contains BNS populations generated with the BSE code for different progenitor metallicities.

Each metallicity subdirectory will contain

`result_fHG0.8.h5`

The directory label `zX` is defined by

```text
X = -log10(Z / Z_sun)
```

so that, for example, `z2.3` corresponds to ($Z = 10^{-2.3} Z_\odot$).

| Directory | Progenitor metallicity |
|---|---:|
| `z0` | ($10^{0} Z_\odot$) |
| `z0.2` | ($10^{-0.2} Z_\odot$) |
| `z0.4` | ($10^{-0.4} Z_\odot$) |
| `z0.6` | ($10^{-0.6} Z_\odot$) |
| `z0.8` | ($10^{-0.8} Z_\odot$) |
| `z1` | ($10^{-1} Z_\odot$) |
| `z1.3` | ($10^{-1.3} Z_\odot$) |
| `z1.8` | ($10^{-1.8} Z_\odot$) |
| `z2.3` | ($10^{-2.3} Z_\odot$) |

## 2. Cosmological BNS merger population

The `Cosmergers/` directory will contain

`result_Cosmergers.h5`

This file contains the paper's **Cosmergers** population: BNS mergers per unit observer-frame time, combining 100 Monte Carlo realizations.

## 3. SKA-detectable Galactic BNS pulsars

The `SKA/` directory contains simulated Galactic BNS pulsars detected with different SKA configurations. Results are organized into `AA4/` and `AAstar/`.

### AA4

- `result_SKA_mid_band1_AA4.h5`
- `result_SKA_mid_band2_AA4.h5`
- `result_SKA_low_AA4.h5`

### AAstar

- `result_SKA_mid_band1_AAstar.h5`
- `result_SKA_mid_band2_AAstar.h5`
- `result_SKA_low_AAstar.h5`

Each SKA data file contains the combined sample from 100 Monte Carlo realizations.

## Data availability

The data products listed above correspond to the **Fiducial** model. Data for the other models are available upon reasonable request to the corresponding author.
