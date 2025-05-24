# Bihar Flood Inundation Panel Dataset (1998–2021)

This repository contains a district-wise panel dataset of flood inundation events in Bihar, India, spanning from 1998 to 2021. The dataset is constructed using satellite-derived flood maps provided by the **National Remote Sensing Centre (NRSC)** and is harmonized with **Socioeconomic High-resolution Rural-Urban Geographic (SHRUG)** data using census-defined district boundaries.

> 📍 **Data granularity:** District-level (as defined by the 2011 Census)  
> 🗓️ **Time span:** Annual data from 1998 to 2021  
> 🌊 **Coverage:** Flood inundation events mapped across all districts of Bihar

## 📡 Data Sources

- **Flood Maps**: Provided by [NSRC](https://bhuvan-app1.nrsc.gov.in/thematic/thematic/index.php), which offers annual flood inundation maps based on satellite imagery. For details on how this mapping is conducted, please refer to their [explainer](https://bhuvan-app1.nrsc.gov.in/bhuvan_links.php#flood).
- **District Boundaries**: Linked to SHRUG and aligned with the 2011 Indian Census (`pc11_district_id`), ensuring consistency for merging with socioeconomic datasets.

## 📁 Dataset Structure

Each row in the dataset represents one district in one year, tracking the extent and frequency of flood inundation.

| Variable                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `index`                | Unique identifier for each row in the dataset                               |
| `year`                 | Year of observation (1998 to 2021)                                          |
| `pc11_district_id`     | Unique district ID as per 2011 Indian Census (used in SHRUG)                |
| `district_name`        | Name of the district                                                        |
| `num_inundation_events`| Number of separate flood inundation events recorded in the district that year |
| `inundated_area_m2`    | Total area (in square meters) inundated by floods during that year          |
| `inundated_area_km2`   | Total area (in square kilometers) inundated by floods (same as above, converted) |

> Note: `num_inundation_events` represents unique inundation episodes rather than days of flooding.

## 🔗 Suggested Use

- Temporal analysis of flood frequency and extent across Bihar
- Merging with SHRUG or other district-level panel datasets for socioeconomic analysis
- Climate vulnerability mapping and disaster risk modeling

## 📜 License

Please cite the original data providers (NRSC, SHRUG) appropriately when using this dataset. This repository is made available for academic and non-commercial use.

---

For any questions, suggestions, or contributions, feel free to open an issue or submit a pull request.
