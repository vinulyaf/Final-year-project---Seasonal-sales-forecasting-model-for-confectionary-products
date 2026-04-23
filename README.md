# Final-year-project-Seasonal-sales-forecasting-model-for-confectionary-products
A Python based project that forecasts regional confectionery sales using seasonal time-series models. Supports demand planning through data analysis, modelling, and forecast evaluation.

Seasonal Sales Forecasting – Sugar Confectionery Segment Project Overview

This project develops a time-series forecasting solution for the sugar confectionery segment using historical monthly sales data. The objective is to predict sales demand by Region and Candy Type to support more accurate baseline demand planning and data driven decision making within the FMCG industry.

The project follows an end-to-end analytics workflow including data preparation, exploratory analysis, forecasting model development, and performance evaluation. Business Problem

Sales in the confectionery sector are highly seasonal and vary significantly across regions and product categories. Traditional forecasting methods based on manual judgement often lead to:

Over-stocking during low-demand periods

Stock shortages during peak seasons

Inefficient inventory and supply chain planning

This project aims to address these challenges by building statistical forecasting models that capture seasonality and trends at a granular level.

Dataset

Monthly sales data from January 2023 – December 2025

Structured at the level of:

Region

Candy Type

Sales Volume

Data was originally provided in wide Excel format and transformed into time-series format for modelling.

Methodology

The project consists of the following key stages:

Data Preparation

Exploratory Data Analysis (EDA)
Trend and seasonality analysis
Forecasting Models Implemented
SARIMA
Holt–Winters Exponential Smoothing
LSTM


Model Evaluation
Train-test split with 80/20

Accuracy measured using Mean Absolute Percentage Error (MAPE)

Model comparison across regions and candy types

Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

Statsmodels

Prophet

Key Outputs

forecasting pipeline

MAPE-based performance comparison tables

Regional and product-level forecasts
