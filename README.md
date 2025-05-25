# Bihar Flood Inundation Panel Dataset (1998–2021)

This repository documents a district-wise panel dataset of flood inundation events in Bihar, India, covering the period from 1998 to 2021. The dataset is built using satellite-derived flood maps provided by the **National Remote Sensing Centre (NRSC)** and is aligned with **Socioeconomic High-resolution Rural-Urban Geographic (SHRUG)** data using 2011 Census district boundaries.

> 📍 **Data granularity:** District-level (as per Census 2011)  
> 🗓️ **Time span:** Annual data from 1998 to 2021  
> 🌊 **Coverage:** Flood inundation events across all districts in Bihar

## 📡 Data Sources

- **Flood Maps**: Obtained from [NRSC](https://bhuvan-app1.nrsc.gov.in/thematic/thematic/index.php), which uses satellite imagery to map annual flood inundation. Learn more about their methodology in [this explainer](https://www.nrsc.gov.in/sites/default/files/pdf/ebooks/Chap_12_FloodDisasterManagement_p1.pdf).
- **District Boundaries**: Derived from the 2011 Indian Census and linked to SHRUG to facilitate integration with socioeconomic data.

## 📁 Dataset Structure

Each row corresponds to a district-year combination, reporting the scale and frequency of flood inundation.

| Variable                | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `index`                | Unique identifier for each row in the dataset                               |
| `year`                 | Year of observation (1998 to 2021)                                          |
| `pc11_district_id`     | District ID as per 2011 Census, used in SHRUG                               |
| `district_name`        | Name of the district                                                        |
| `num_inundation_events`| Number of distinct flood inundation events recorded in the year             |
| `inundated_area_m2`    | Total area inundated (in square meters)                                     |
| `inundated_area_km2`   | Total area inundated (in square kilometers)                                  |

> `num_inundation_events` refers to distinct episodes, not total days of flooding.

## 🤝 Collaboration

I’m actively looking for opportunities to collaborate and explore this dataset further—whether that’s through joint research, policy engagement, or technical development.

**If you're interested in working with this dataset, please feel free to reach out via email: [taha.i.siddiq@gmail.com](mailto:taha.i.siddiq@gmail.com)**

## 📜 License & Access

The dataset is not publicly available at this time. Access can be granted upon request for collaborative purposes. Please ensure proper attribution of original sources (NRSC, SHRUG) when using or referencing the data.

---
