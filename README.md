Here, we make the supplemental materials for our publications available on github.

Anyone can send email to me: binliuhy@tsinghua.edu.cn

## Dataset Overview

| Total configurations | 2,077 |

## Configuration Types

The dataset covers four types of atomic configurations:

| Configuration Type | Count | Percentage |
|-------------------|-------|------------|
| Bi₂Te₃/Sb₂Te₃ interface & Bi_x Sb_{2-x}Te₃ alloy | 759 | 36.5% |
| Bulk Bi₂Te₃ | 677 | 32.6% |
| Bulk Sb₂Te₃ | 600 | 28.9% |
| Other | 41 | 2.0% |

## Structure Statistics

### Atom Count Distribution

| Atoms per Config | Count | Percentage | Description |
|------------------|-------|------------|-------------|
| 240 | 1,418 | 68.3% | Standard 4×4×1 supercell |
| 256 | 339 | 16.3% | Interface/alloy structures |
| 304 | 320 | 15.4% | Extended interface structures |

### Element Statistics

| Element | Total Atoms |
|---------|-------------|
| Bi | 110,630 |
| Sb | 99,786 |
| Te | 313,968 |

### Energy Statistics

| Property | Value |
|----------|-------|
| Energy range | -1210.35 to -883.46 eV |
| Energy per atom | -4.32 to -3.68 eV/atom |
| Mean energy per atom | -3.97 eV/atom |

## Sampling Conditions

- **Temperature range**: 50–600 K
- **Strain perturbations**: ±3% uniform cell scaling
- **Atomic perturbations**: Gaussian noise with σ = 0.1 Å
- **Sampling method**: NPT + NVT ensemble MD with NEP89 universal potential
- **Active learning**: Farthest point sampling (FPS) in descriptor space

## DFT Calculation Parameters

| Parameter | Value |
|-----------|-------|
| Exchange-correlation | PBE-GGA |
| Pseudopotential | PAW |
| Dispersion correction | DFT-D3 |
| Plane-wave cutoff | 400 eV |
| k-points | Γ-centered 1×1×1 |
| Energy convergence | 1×10⁻⁶ eV |
