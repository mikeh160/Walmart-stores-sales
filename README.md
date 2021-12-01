# Walmart-stores-sales
A comprehensive notebook on kaggle competition m5-forecasting-accuracy detailing eda and time series analysis along with forecasting using sarimax and prophet models

## Table of Contents
1. [Project Motivation](#motivation)
2. [File Descriptions](#files)
3. [Instructions](#instructions)
4. [Results](#results)
5. [Licensing, Authors & Acknowledgments](#licensing)

## Project Motivation<a name="motivation"></a>

The project was chosen to experience the complexities that are involved in making timebound forecast,  and also help present a solution to the kaggle comeptition of the namesake M5-Forecasting Accuracy. The project includes a comprehensive exploratory data analysis, time series analysis, and time series forecast. The forecasts were made using the timeseries models SARIMAX and Facebook developed Prophet Model. The final submission file was prepared using the facbook prophet model to make a forecast of number of units sold for each of the individual product ids. 



## File Description<a name="files"></a>

These are three data input files, with one submission file that has to be filled with sales of units predictions for the next 28 days, represented in the submission file as F1,F2 ...F28. 

```
1. sales_train_validation.csv               -file containing categorical level data for about 30,000 unique product ids with number of units sold on almost 1900 days
2. sell_prices.csv                          -file containing some 6 million entries of product prices along item_category distribution
3. calendar.csv                             -file containing date level information along with SNAP (supplementary nutrition assistance programme)
4. submission.csv                           -file containing almost 60,000 product ids (30,000 unique) with validation & evaluation distribution and 28 days columns

5. Comprehensive-eda-sarimax-prophet-forecsating.ipynb            -jupyter file containing all the analysis along with code and detailed explanations
6. packages_installed.txt                   -file containing the packages and the versions that were used to run this project

```

## Instructions<a name="instructions"></a>

In order to run the project place the files in the same directory. The libraries used along with the versions are made available in the file packages_installed.txt file. The data files are kept in the data directory. Or change the path as necessary

## Results<a name="results"></a>

The project provides a detailed overview and a tutorial on exploratory data analysis, time series analysis and the requirements that need to be satisfied before beginning the time series analysis. The modules should be pretty easy to understand, and explanations along with code blocks and from visualizations should make it easier to follow along. Each of the code block deals with answering the questions posed in the beginning of the notebook under the heading, problem statement.

Once requisite questions on understanding the distribution of data were answered, it was time to conduct time series analysis. Again, simple modules were made so that people looking to replicate code blocks for own their usage in the kaggle kernel could just simply copy/paste the modules and may even extend on these to make better and more vivid visulizations. 

In the end, timeseries forecasting was made using SARIMAX and Prophet Models. The requirements that need to be assessed before making the time series analysis were discussed and followed along, along with estimating the parameters using the graphical measurements. Once the parameters were obtained, they were fed into the SARIMAX model. The validation and testing procedures were also presented and visulizes separately to diffrentiate the behavior and the reasoning used behind each of the representations. Similarly, for prophet forecast same procedure was followed to make future forecast along with validation steps. However, in order to make the final submission file more accurate , another prophet model forecast was devised that could make forecasts with any number of product ids specified. But since the prediction for some 30,000 product ids would take considerable time, results and submission file were made using some 1500 unique product ids. The results for remaining product ids were collated using a simple moving average, and the final submission file was prepared by concatinating the results of two predictions.


## Licensing, Authors & Acknowledgments<a name="licensing"></a>

Incredibly grateful to the team at Udacity, Kaggle & Kaggle Community as well as University of Nicosia for providing the data and resources to help complete this project
