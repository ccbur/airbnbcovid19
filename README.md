# AirBNB COVID-19 analysis

## Motivation

This project is giving some insight how COVID-19 impacted Airbnb in **Seattle**. It analyses data from January 2019 to June 2020 and highlights some interesting
effects of COVID-19 to listings, availability and pricing on airbnb.com.

## Quick start
### Requirements
* Python 3.x

### Packages
`pip install numpy pandas seaborn sklearn matplot`

### Repository
`git clone https://github.com/ccbur/airbnbcovid19`

### Run

Open *airbnbcovid.ipynb* in your favorite Jupyter notebook application (Jupyter notebook, Visual Studio Code, Spyder, etc.). At least 8 GB of RAM is needed to run this notebook.

## Results
Questions
- What was the impact of Covid-19 to Airbnb bookings in Seattle?
    June 2019 vs. June 2020
    - Drop in listings: ~33%
    - Drop in official pricing: ~7%
    - Drop in adjusted pricing: ~9%
    - Drop in utilization: ~7%

    **>> COVID-19 has a significant impact on Airbnb listings!**

- Who is offering a COVID-19 deep cleaning?
    Correlation (Hamming distance) between COVID-19 deep cleaning and...
    - ... availability: 0.35
    - ... bedrooms: 0.13
    - ... cal_adjusted_price30: 0.00

    **>> COVID-19 deep cleaning is related to bigger listings with a bad utilization, but no correlation with pricing found**

- Is a COVID-19 deep cleaning offering helpful for landlords to get a better utilization?

    March 2020 - June 2020
    - Change in mean availability without COVID-19 deep cleaning: -0.205017
    - Change in mean availability with COVID-19 deep cleaning: -0.203608

    **>> The offering of COVID-19 deep cleaning is increasing, but the utilization is changing the same as with the listings without deep cleaning.**

## Files
File | Description
------------ | -------------
*README.md* | this README
*airbnbcovid.ipynb* | Jupyter notebook to analyse the airbnb data
*data/20xxxxxx/listings.csv.gz*<br/>*data/20xxxxxx/calendar.csv.gz* | airbnb listings / calendars for Seattle scraped on a specific date (source: http://insideairbnb.com/get-the-data.html)

## License
The code is licensed under the [GNU General Public License v3.0](https://github.com/ccbur/airbnbcovid19/LICENSE).

## Acknowledgements
Thanks to Airbnb for the data.