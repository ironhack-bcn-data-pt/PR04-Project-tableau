![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

*Veronica Agnolutto*

*Data_Barcelona_june .2o*

# Project: Evolution of Covid19 (Spain)

## Project description

The goal of this project was to practice what we have learned in **Module 2**. The idea was to combine **python** programming with **time series** and **interactive maps**.

## Goal

General analysis of the **evolution of Covid19 in Spain** from March to October 2020 and **localization of the healthcare facilities** available for installing future Covid19 modules.

---

## Data

The dataset we are working with are two:

- **CNH_2019.xls** : Healthcare facilities in Spain
- **covid19-provincias-spain_consolidated.csv**: Covid19 cases

## Organization

The following deliverables should be pushed to your Github repo for this chapter.

* **PR05-Covid_evolution_Spain.ypynb**: working file
* **input folder**: contains the original datasets
* **output**: contains modified datasets useful for the visualizations
* **gitignore**

## Lessons learned

* Loading Datasets with multiple sheets
* Geocoding
* Time series (Rolling mean)
* Interactive maps

## Obstacles
* Geocoding (Nominatim doesn't recognize addresses of the healthcare structures)
* TimeSliderChoropleth

## Possible future improvements
* Location allocation analysis (Identifying suitable sites for new Covid clinics)
* Widgets in the timeseries graph

## Links

[Repository](https://github.com/cucu-o0/PR05-project-tableau)
