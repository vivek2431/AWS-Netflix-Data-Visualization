# AWS Netflix Data Visualization Project

## Overview

This project uses Amazon QuickSight to visualize data from a Netflix database. The visualization includes various graphs and charts to create a comprehensive dashboard.
The project demonstrates the use of AWS services such as S3 and QuickSight to process and analyze large datasets efficiently.

![architecture-diagram](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/2e8d3c82-3421-4479-a6ea-6967c8b21fe2)

![42](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/e8cd5d11-fef3-47c7-ba65-54f7a9078923)




## Table of Contents

- [Introduction](#introduction)
- [Project Setup](#project-setup)
  - [Upload Data to S3](#upload-data-to-s3)
  - [Create QuickSight Account](#create-quicksight-account)
  - [Connect S3 to QuickSight](#connect-s3-to-quicksight)
- [Data Visualization](#data-visualization)
  - [Creating Visualizations](#creating-visualizations)
  - [Using Filters](#using-filters)
  - [Setting Up Dashboard](#setting-up-dashboard)
- [Key Learnings](#key-learnings)
- [Author](#author)

## Introduction

Amazon QuickSight is a scalable, serverless business intelligence service provided by AWS. It offers fast, easy-to-use data visualization, interactive dashboards, and integrated machine learning insights. This project leverages Amazon QuickSight to visualize Netflix data, enabling insights through graphical representations.

## Project Setup

### Upload Data to S3

#### Store the Dataset in Amazon S3

- Log in to your AWS Account.
  
- Open your S3 console.

- Select Create Bucket.

  ![1](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/d4a93705-34a2-4a8d-b7f8-ce3e5b30b47c)


💡 Why are we using Amazon S3? Isn't this project about QuickSight?
In this step, we're storing our dataset in an Amazon S3 bucket. Later, QuickSight will connect to S3 to use the data in this bucket and create visualisations.

- Name the bucket nextwork-quicksight-project-name (replace name with your name).

  ![2](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/d1f3c4fc-d979-4629-bb44-e71d4b4dc03f)

- Select the Region closest to you.
  
- Keep the rest of the settings as default, and select Create bucket.

  ![4](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/21f34e1f-c914-4bd0-a0cb-680383f1c7c6)

- Upload the CSV file and the manifest.json file into the bucket.
  
- Copy the S3 URL of your netflix_titles.csv file.

  ![6](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/4fcfae44-8d3b-4a95-94c3-3ea1f7eb1ac6)

 ![9](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/c806ffdb-12f4-4a04-a7f0-ed82d905f64d)


- ✍️ Documentation time: head to the slide titled Upload your dataset and a manifest.json file into S3 in your documentation template, and fill in the first prompt!
- S3 is used in this project to store my dataset and
  manifest.json file
- I edited the manifest.json file by updating the S3 URI of
  my dataset. It’s important to edit this file because
  keeping an outdated S3 URI means that manifest.json
  would be directing to the wrong address.

 Open your manifest.json file in your laptop's text editor - for example, TextEdit (Mac) or Notepad (Windows).
 Replace the URL in the manifest.json file with the S3 URL of your dataset.

 ![7](https://github.com/vivek2431/AWS-Netflix-Data-Visualization/assets/137812531/260715e4-dc18-44fa-9a31-933ac8f27dd9)

### Create QuickSight Account

1. **Sign Up for QuickSight**: Create a free QuickSight account (free trial lasts for 30 days).
2. **Enable S3 Access**: Grant QuickSight access to your S3 bucket to allow it to process the dataset.

### Connect S3 to QuickSight

1. **Configure QuickSight to Access S3**: Use the S3 URL of the `manifest.json` file to connect QuickSight to the S3 bucket.
2. **Verify Connection**: Ensure that QuickSight can access and process the data files as specified in the `manifest.json` file.

## Data Visualization

### Creating Visualizations

1. **Autograph Space**: Drag relevant fields into the QuickSight dashboard's Autograph space.
2. **First Visualization**: Create a graph showing a breakdown of movies and TV shows for every release year by placing the release year on the y-axis and grouping by type (movie or TV show).

### Using Filters

1. **Apply Filters**: Exclude data irrelevant to your analysis. For example, filter out movies and TV shows released before 2015.
2. **Custom Visualization**: Focus on movies and TV shows of specific genres released from 2015 onwards.

### Setting Up Dashboard

1. **Edit Titles**: Clarify the purpose of each chart by editing the titles.
2. **Export Dashboard**: Publish the dashboard and export it as a PDF for sharing or presentation.

## Key Learnings

1. **S3 Integration**: Using an S3 bucket to store data files facilitates seamless integration with QuickSight.
2. **Efficient Visualization**: QuickSight's intuitive interface and built-in features make generating insightful visualizations straightforward.
3. **Performance**: QuickSight efficiently processes and visualizes large datasets, enabling the creation of detailed dashboards quickly and effortlessly.

## Author

[Vivek Singh](https://linkedin.com/in/viveksingh2303)

For more information, visit [NextWork](http://www.nextwork.org/).
