
# Formula 1 pit stop time Effect on races

-   author: Flora Ouedraogo
-   contributors: Flora Ouedraogo

Demo of a data analysis project for DSCI 522 (Data Science workflows); a course in the Master of Data Science program at the University of British Columbia.

## Introduction

For this project we are trying to answer the question: Does the pit time stop affect the race results? Answering this question is very important in understanding the different factors that play in winning a Grand Prix. Indeed, most of the time, the pit stop time factor is omitted by the drivers and the constructors whenever they give the reasons why they won or not a race. Most drivers will point at the weather conditions, the engine, the teamwork, their good shape; but rarely, they will mention how the pit stop time. This project will help us know if the time spent on the pit can be an important factor of winning a race.

The data set used in this project is the Formula 1 World Championship datasets from 1950 2021 published on the Kaggle website. The Formula 1 World Championship datasets comprises several data collected about this industry. They are: circuits.csv, constructor_results.csv, constructor_standings.csv, constructors.csv, driver_standings.csv drivers.csv , lap_times.csv, pit_stops.csv, qualifying.csv, races.csv, results.csv, seasons.csv, status.cs. for the purpose of this study we will focus on the pit stop data.

Each row in the data set represents summary statistics of the pit stop, and this includes the lap number, the duration of the stop, and the driver id.

To answer the inferential question posed above, we plan to carryout the analysis in R. The analysis will start by exploring the data distribution, then, we will choose a suitable estimator given the question mentioned above and the data we have from Kaggle. Another important part of our alaysis would be to specify the hypotheses and the test flavor. Lastly, we will interpret the results.

Thus far we have performed some exploratory data analysis, and the report for that can be found [here](src/pit_stop.md).

## Usage

To replicate the analysis, clone this GitHub repository, install the [dependencies](#dependencies) listed below, and run the following commands at the command line/terminal from the root directory of this project:

    python src/download_data.py --out_type=pit_stops --url=https://www.kaggle.com/rohanrao/formula-1-world-championship-1950-2020--out_file=data/raw/formula1
    Rscript -e "rmarkdown::render('src/formula_1.Rmd')"

## Dependencies

-   Python 3.9.5 and Python packages:

    -   docopt==0.6.2
    -   requests==2.25.1
    -   pandas==1.3.2

-   R version 3.6.1 and R packages:

    -   knitr==1.33

    -   tidyverse== 1.3.1

## License

Formula 1 pit stop time Effect on races here are is the intellectual property of FO. If re-using/re-mixing please provide attribution and link to this webpage.

# References
