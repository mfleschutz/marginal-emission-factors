⚠ The latest version of the repository lives in the DrafProject organisation: https://github.com/DrafProject/marginal-emission-factors

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4718362.svg)](https://doi.org/10.5281/zenodo.4718362)

# marginal-emission-factors
This directory provides updatable supplementary data to the journal paper [Fleschutz et al. (2021)](https://doi.org/10.1016/j.apenergy.2021.117040).

The time series were calculated in hourly resolution (`data/60min`), and were additionally converted to quarter-hourly resolution (`data/15min`).

## Data description
| Column name   | Data type | Unit            | Description     |
| ------------- |-----------| --------------- | ----------------|
| T             | Integer   | Hour/Quarterhour| Hour/Quarterhour of the year starting with `0`. |
| residual_load | Float     | MW_el           | Average residual national load. |
| total_load    | Float     | MW_el           | Average total national load. |
| marginal_fuel | String    | -               | Fuel type of marginal power plant. One of `lignite`, `coal`, `gas`, `gas_cc`, and `oil`. |
| efficiency    | Float     | -               | Efficiency of marginal power plant between 0 and 1. |
| marginal_cost | Float     | € / MWh_el      | Marginal cost of electricity generation. |
| MEFs          | Float     | kg_CO2eq/MWh_el | Marginal emission factors. I.e. the carbon emission intensity of electricity generation of the marginal power plant. |
| XEFs          | Float     | kg_CO2eq/MWh_el | Average electricity grid mix emission factors. |

## License
Data is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

## How to cite this data
If you use this data, please cite the journal paper [Fleschutz et al. (2021)](https://doi.org/10.1016/j.apenergy.2021.117040) or the [zenodo repository](https://doi.org/10.5281/zenodo.4718362).
