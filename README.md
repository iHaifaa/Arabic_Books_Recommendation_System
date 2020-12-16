# Arabic_Books_Recommender
The capstone project for Data Science, Immersive course by Misk Academy. 

Haifaa Alzahrani

10/12/2020

## Overview
Developing recommendation systems is one of the promising applications of data science. However, investigating the Arabic language in relation to developing reliable recommendation systems remains a major challenge. For example, it suffers from the absence of reliable datasets in this domain. Besides, processing Arabic texts has its own obstacles due to the nature of the language itself (), differences in dialects, and thus we have very few efforts to overcome these issues and investigate Arabic-based recommendation systems compared to English.

## Objectives
The main objectives of this project are: 

1. Providing a dataset for Arabic books. 

2. Developing an NLP-based recommendation system for Arabic books by applying a text similarity algorithm. 


## Notebooks Description
This project consists of the following notebooks:

1. **Books_Scraper**
This scraper fetches Arabic books data from [Abjjad](http://abjjad.com) website by 2 methods. The input and output of this process are provided in [Data/Lists_of_Links](https://github.com/iHaifaa/Arabic_Books_Recommendation_System/tree/main/Data/Lists_of_Links), and [Books_Data](https://github.com/iHaifaa/Arabic_Books_Recommendation_System/tree/main/Data/Books_Data) folders.

2. **Dataset_Preparation**
This notebook aims to create 2 separated datasets for general data science projects and NLP-based projects. They are available in [Data/Books_Data](https://github.com/iHaifaa/Arabic_Books_Recommendation_System/tree/main/Data/Books_Data) folder.

3. **EDA**
Very basic EDA for **Prepared_Dataset.csv**. The plots are saved in [Plots](https://github.com/iHaifaa/Arabic_Books_Recommendation_System/tree/main/Plots) folder.

4. **Pre-processing**
This notebook is used to pre-process **Descriptions_Dataset.csv** to prepare it for the recommendation system. 

5. **Books_Recommender**
Here, we used AraVec (word embedding for Arabic texts) with Cosine Similarity to build our recommendation system.

## Dataset Description
The dataset is scraped from [Abjjad](http://abjjad.com) website. It is the first public dataset for Arabic books. In addition, it is the first one to include books description texts in Arabic. The dataset comes in 2 different files: 

1. **Prepared_Dataset.csv**, which consists of the books with their metadata including the description texts, for general use. 

2. **Descriptions_Dataset.csv**, which only consists of the books with their description texts, to NLP-based projects.

You will find them in [Data/Books_Data](https://github.com/iHaifaa/Arabic_Books_Recommendation_System/tree/main/Data/Books_Data) folder.

The description of the features as the following: 

| Feature | Description |
|:----------------:|:----------------------------------------------------------------------------------------------:|
| ISBN | ISBN or ISBN 13 of the book. |
| Title | The whole title of the book. |
| Author | The author name/s. Like the main author, co-author, and translator. |
| Authors_Number | Number of authors, it is 1 if the book has only one author. |
| Description | The text description of the book, taken from the book summary or written by an admin. |
| Genres | The category of the book. |
| Average_Ratings | Average rate for a given book. |
| Reviews_Number | Number of written reviews by users. |
| Quotes_Number | Number of quotes taken from the book and published by users. |
| Community_Size | Number of users who added the book to their shelves (as read, currently reading, or to_read) |
| Pages_Number | Amount of pages per title. |
| Editions | Number of different editions for the book, not the current one. |
| Publication_Year | Year of the first publication. |
| Publisher | Publisher's name. |
| URL | Direct link to the book's page on Abjjad. |
| Cover_URL | Direct link to the book's image on Abjjad. |


## Notes
 This project includes a couple of different modules, so you have to install them before running this project.
