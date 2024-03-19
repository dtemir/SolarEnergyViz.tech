![huiowa23Engie](https://socialify.git.ci/kboytron/huiowa23Engie/image?description=1&font=Bitter&logo=https%3A%2F%2F1000logos.net%2Fwp-content%2Fuploads%2F2021%2F03%2FEngie-logo.png&name=1&theme=Light)

# SolarEnergyViz.tech 
## Engie challenge for HackUIowa , with sprinkes of GitHubOps, DevOps, and WebDev.
This project was made to investigate the differences between triple-junction amorphous and poly-crystalline solar panels, and to inform people about the potential benefits of switching to solar energy. The links above provide a calculator that estimates the potential profit of switching to solar, a comparison between the 2 types of solar panels, and a compilation of the last 10 years of data collected by existing solar panels in the University of Iowa's Electric Vehicle Charging Array.

![overview](https://github.com/dtemir/SolarEnergyViz.tech/assets/62047062/be1afa3b-c60e-49f5-a23d-a9087b6ccfee)

# 🔑 Key Feature
## Calculates how much money you can make by being sustainable
<img src="https://i.imgur.com/g2fhJyt.png" width=85%>

## Trains a time-series prediction model to predict future solar irradiance (fill the gap for 2021 - 2023) & Compares conversion efficiency of two different solar arrays
<img src="https://i.imgur.com/nkVIxrS.png" width=65%>

## Visualizes 12 years worth of Conversion Efficiency
<img src="https://i.imgur.com/2PoEbs0.png" width=65%>

## Automatically Cleans the solar panel dataset, excluding erroneous and arbitrary values
<img src="https://i.imgur.com/0X5u5Td.png" width=65%>

# 🏆Personal Accomplishments that I'm proud of
- Worked with pandas library and learnt a lot of new things
- Managed to perform data cleaning on 10 years worth of solar panel data
- Performed necessary data restructuring using Pandas

## 🛠 Skills
Data cleaning, data visualization, pandas, python , prophet (time series prediction), html , css , matplotlib

# 📃 Challenges we faced

## Missing Values

- Some of the data wasn't clean. 
- We found missing variables, such as `Calc Failed` and `[-11059] No Good Data For Calculation`.
- For `Calc Failed`, we calculated the value by adding daily hours into totals.
- For `[-11059] No Good Data For Calculation`, we used that day's total, subtracted all of the other hours, and split the difference among the hours that had that value.

## Extremely High Values

- Some of the data provided contained very high values, such as `2.38572E+30`. We made sure to filter that data out as to not skew calculations.
- All of that data seem to happen during night-time when the kWH records would have been very low. 

## NSRDB not accounting for tilt, azimuth

The NSRDB data does not account for tilt and azimouth of the array as well as max generation capacity. To account for the difference in installation, we relied on the [PVWatts calculator](https://pvwatts.nrel.gov/pvwatts.php) to find the ratio of change. The data we observed with the arrays:

| Month  | EV Solar Radiation (kWh / m^2 / day)  | CAMBUS Solar Radiaton (kWh / m^2 / day) | Difference |
|---|---|---|---|
| January | 4.11  | 2.53  | 1.58 |
| February  | 4.79  | 3.23  | 1.56 |
| March  | 5.71  | 4.25  | 1.46 |
| April  | 6.22  | 5.02  | 1.2 |
| May  | 6.71  | 5.83  | 0.88 |
| June  | 7.26  | 6.43  | 0.83 |
| July  | 7.74  | 6.60  | 1.14 |
| August  | 7.31  | 5.98  | 1.33 |
| September  | 6.74  | 4.99  | 1.75 |
| October  | 5.39  | 3.62  | 1.77 |
| November  | 3.87  | 2.47  | 1.4 |
| December  | 3.17  | 1.99  | 1.18 | 

<details> 
  <summary>PVWatts calculator for EV Charging Array </summary>
  <img width="1013" alt="image" src="https://github.com/kboytron/huiowa23Engie/assets/62047062/87054fbb-1602-4103-9751-1fbbe0bd1f99">
  <img width="1000" alt="image" src="https://github.com/kboytron/huiowa23Engie/assets/62047062/18d3a3ff-3783-45b6-9dc3-0f6431f6434f">
</details>

<details> 
  <summary>PVWatts calculator for CAMBUS Array </summary>
  <img width="1016" alt="image" src="https://github.com/kboytron/huiowa23Engie/assets/62047062/9edf98f5-fbdd-42a2-bb5c-14b10bd0d34c">\
  <img width="996" alt="image" src="https://github.com/kboytron/huiowa23Engie/assets/62047062/cdc7f3f8-d656-4593-a699-c53c7fa6cc5e">
</details>

# Meet The Team
  - <a href="https://github.com/kboytron">Karan Singh</a>
  - <a href="https://github.com/NolanScherer">Nolan Scherer</a>
  - <a href="https://github.com/dtemir">Damir Temir</a>
  - <a href="https://github.com/Saitarun994">Sai Tarun Sathyan</a>