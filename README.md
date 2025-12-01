CORD-19 Research Metadata Analysis & Streamlit Dashboard
1. Project Overview

This project explores the CORD-19 research metadata, which contains thousands of COVID-19–related research papers.

The goal is to:

Load and clean the dataset

Analyze publication trends, journals, and sources

Generate visual insights

Build an interactive Streamlit dashboard to explore the data

2. Dataset

File used: metadata.csv (sample of 10,000 rows for faster processing)

Key columns:

title: Paper titles

abstract: Paper abstracts

publish_time: Date of publication

journal: Publishing journal

source_x: Source repository (PMC, medRxiv, bioRxiv, WHO)

3. Installation

To run this project locally:

Clone the repo:

git clone <your-repo-url>
cd Frameworks_Assignment


Install required packages:

pip install pandas matplotlib seaborn streamlit wordcloud


Run the Streamlit dashboard:

streamlit run app.py

4. Features

Data Preview: View the first few rows of the dataset

Year Filter: Interactive slider to select a range of publication years

Publications Over Time: Bar chart showing number of papers per year

Top Journals: Bar chart of the top 10 publishing journals

Word Cloud: Most frequent words in paper titles

Filtered Table: Preview of papers based on selected year range

5. Visualizations

Publications per Year: Trend showing research activity over time

Top Journals: Journals with the highest number of publications

Word Cloud of Titles: Highlights most common words in paper titles

Source Distribution: Number of papers per source (PMC, medRxiv, etc.)

6. Challenges

Dataset is large → Used a smaller sample (metadata_sample_10k.csv)

Missing publication dates → Converted to datetime with errors='coerce'

Streamlit cannot run directly in Colab → Used LocalTunnel to expose the app

Some abstracts or titles missing → Handled with placeholder text

7. Learning Outcomes

Hands-on experience with pandas for data cleaning and analysis

Creating visualizations with matplotlib, seaborn, and WordCloud

Building an interactive dashboard with Streamlit

Experience with filtering, summarizing, and exploring real-world data

8. Live App

You can view the Streamlit dashboard online here:

https://salty-adults-own.loca.lt

9. Repository Contents
Frameworks_Assignment/
│
├── metadata.csv              # Sample dataset
├── app.py                    # Streamlit dashboard
├── analysis.ipynb            # Notebook with full analysis and visualizations
├── README.md                 # Project documentation
└── figures/                  # Opti
