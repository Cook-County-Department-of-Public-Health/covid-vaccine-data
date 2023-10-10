# Cook County Department of Public Health COVID-19 Vaccination Data Repository

## Background

This repository was created to share data related to COVID-19 vaccination coverage among residents living in the Cook County Department of Public Health's jurisdiction. Our jurisdiction covers Cook County, except areas that have their own state-certified local health department. These places include the cities of Chicago, Evanston, Oak Park, Skokie, and Stickney township.

Vaccination data for our jurisdiction comes from the Illinois Comprehensive Automated Immunization Registry Exchange, or [I-CARE](https://dph.illinois.gov/topics-services/prevention-wellness/immunization/icare.html), a web-based immunization registry operated by the Illinois Department of Public Health. Reporting immunizations to I-CARE is typically voluntary. However, during the COVID-19 Public Health Emergency, vaccination providers received vaccines from the federal government at no cost. In exchange for these supplies, providers committed to reporting administered COVID-19 vaccinations to their state immunization registries. As a result, vaccination coverage could be estimated using these data.

With the ending of the Public Health Emergency declaration on May 11, 2023, COVID-19 vaccines will [commercialize](https://aspr.hhs.gov/COVID-19/Pages/FAQ-Commercialization.aspx); when the federal government's current supply of vaccines is exhausted, procurement and payment will move to traditional pathways and **vaccinations will no longer be reportable** to I-CARE. This transition is currently expected in early fall of 2023. This repository will continue to be updated on a monthly basis; however, we expect coverage estimates to be **less accurate** following the transition to commercial pathways and voluntary provider reporting to I-CARE. 

## How to Use This Repository

This repository contains comma separated values (CSV) files of data. If you are unfamiliar with this type of file, you can open, view, and edit it using Microsoft Excel, Google Sheets, or other software.

To download all of the data in the repository, click the green button labeled “Code” at the top of this page. Clicking this button will allow you to download a ZIP file of the entirety of the data.

To download a single file, click on the file you would like to download. You will see the data in CSV format. From there, click the “Raw” button. Right click, and select to save the file as a CSV.

## Contents

* **vaccine-weekly-totals**: This file contains weekly cumulative counts and coverage estimates for CCDPH's jurisdiction.
* **vaccine-weekly-by-age**: This file contains weekly cumulative counts and coverage estimates for CCDPH's jurisdiction, broken down by age group.
* **vaccine-weekly-by-race-ethnicity**: This file contains weekly cumulative counts and coverage estimates for CCDPH's jurisdiction, broken down by race and ethnicity group.
* **vaccine-weekly-by-district**: This file contains weekly cumulative counts and coverage estimates for CCDPH's jurisdiction, broken down by our four public health [districts](https://cookcountypublichealth.org/wp-content/uploads/2018/12/SCC-Map.pdf).

## Definitions

Files contain the number of residents with at least one dose of any COVID-19 vaccine (n_onedose), the number of residents with at least one 2022 (bivalent) shot (n_bivalent), and the number of residents with an updated 2023-2024 shot (n_2023). Residents are considered "up to date" with COVID-19 shots if they have received an updated 2023-2024 vaccine. Current vaccine recommendations are available [here](https://www.cdc.gov/coronavirus/2019-ncov/vaccines/stay-up-to-date.html). Coverage estimates for all measures are calculated by dividing the number of residents vaccinated by the corresponding population estimate from the 2020 Decennial Census, then multiplying by 100 to obtain a percent.

For n_onedose and coverage_onedose, data are grouped by the earliest shot date on record. For n_bivalent and coverage_bivalent as well as n_2023 and coverage_2023, data are grouped by the earliest date of 2022 (bivalent) or 2023-2024 booster receipt, respectively. 

## Caveats

Numbers in these files are considered estimates. They are provisional and subject to change. Vaccinations given out of state are not included in I-CARE. Some providers may not comply with reporting requirements, resulting in missing vaccinations, or may report demographic data incorrectly. 

Conversely, some patients' shot records may not be appropriately linked causing shots to be split across multiple duplicate patient records. We attempt to correct these instances by matching shots on both I-CARE ID, as well as name and date of birth. 

## Additional Data

For other data not presented in this repository, please complete an External Data Request [Form](https://cookcountypublichealth.org/epidemiology-data-reports/data-request-forms/).
