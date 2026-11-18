# Data

| File | Content |
|---|---|
| `features_clean.csv` | One row per grid cell (1,659 rows): identifier, centre coordinates, governorate, solar, population, land-cover and distance variables, and the transformed features |
| `clustered_cells.csv` | The same table with the K-Means cluster of each cell |
| `cluster_profiles.csv` | Mean of each feature per cluster |
| `model_comparison.csv` | Scores of the six clustering models |
| `shortlist.csv` | Eligible cells with their top-100 frequency |

Raw data are not stored in this repository. They are large and have their own licences; download them from the sources listed in the main README.

## Main columns

| Column | Meaning | Unit |
|---|---|---|
| `cell_id` | Grid cell identifier | |
| `lon`, `lat` | Centre of the cell (WGS84) | degrees |
| `governorate` | Governorate with the largest overlap | |
| `PVOUT` | Specific photovoltaic output | kWh/kWp per year |
| `GHI`, `DNI` | Global horizontal and direct normal irradiation | kWh/m² per year |
| `pop_density` | Inhabitants per square kilometre | people/km² |
| `pct_builtup`, `pct_cropland`, `pct_bare`, `pct_water`, `pct_tree_shrub_grass` | Land-cover shares | % |
| `dist_road_km`, `dist_power_line_km`, `dist_substation_km` | Distance from the cell centre to the nearest feature | km |
| `log_*` | Natural logarithm of one plus the variable | |

## Credits

Global Solar Atlas 2.0 (World Bank Group, ESMAP, Solargis, CC BY 4.0); WorldPop; ESA WorldCover 2021 v200; © OpenStreetMap contributors (ODbL); geoBoundaries.
