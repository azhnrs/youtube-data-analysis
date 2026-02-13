📊 YouTube Video Data Analysis using YouTube Data API v3

📌 Overview

This project analyzes YouTube video metadata collected using the YouTube Data API v3.
The goal is to explore video performance trends based on views, likes, comments, and publication date.

The project covers the complete data pipeline:

Data collection from API

Data cleaning & preprocessing

Data aggregation

Time-series analysis

Data visualization

🎯 Objectives

Collect YouTube video data programmatically using API

Perform structured data preprocessing

Analyze engagement metrics (views, likes, comments)

Explore time-series trends by category

Visualize video performance patterns

📂 Dataset Information

Data Source: YouTube Data API v3

Time Range: January 1, 2023 – November 30, 2023

Total Videos Collected: 500

Stored as: youtube_data.csv

Extracted Fields:

videoId

title

description

publishedAt

categoryId

viewCount

likeCount

commentCount

tags

⚙️ Data Processing Steps
1️⃣ Data Collection

Retrieved video metadata using YouTube Data API v3

Extracted up to 500 videos within the specified date range

Saved raw data into CSV format

2️⃣ Data Cleaning & Preprocessing

Loaded dataset into Pandas DataFrame

Checked data types and missing values

Dropped tags column (all values missing)

Filled missing values:

description → "description not available"

likeCount → 0

commentCount → 0

Converted publishedAt to datetime format

Set publishedAt as DataFrame index

3️⃣ Data Aggregation

Grouped data by:

Publication date (daily)

Video category

Aggregated metrics:

Total views

Total likes

Total comments

4️⃣ Data Visualization

Visualized time-series trend of daily views

Focused on Category 1 as sample analysis

Used Matplotlib for visualization

📊 Sample Analysis Insight

Daily engagement trends show fluctuation based on upload activity

Certain days exhibit significant spikes in views

Engagement metrics (likes & comments) correlate with view volume

(You can insert screenshot of the visualization here)

🛠 Technologies Used

Python

YouTube Data API v3

Pandas

Matplotlib

NumPy
