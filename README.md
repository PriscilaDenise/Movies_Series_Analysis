

# Streaming Content Analysis

## Overview
This project analyzes a dataset of streaming content to uncover trends in genres, platforms, and original content performance. The analysis is conducted in a Jupyter Notebook (`Streaming_Content_Analysis.ipynb`) using Python, with visualizations including bar graphs for genre and platform distributions and a word cloud for content tags. The dataset (`streaming_content_dataset.csv`) contains information on streaming titles, including genres, platforms, release years, viewer ratings, and more.

## Dataset
The dataset (`streaming_content_dataset.csv`) includes the following columns:
- **Content_ID**: Unique identifier for each title.
- **Title**: Name of the movie or show.
- **Type**: Movie or TV series.
- **Genre**: Primary genre (e.g., Drama, Action, Comedy).
- **Platform**: Streaming platform (e.g., Netflix, Disney+, HBO).
- **Release_Year**: Year of release (converted to Int64).
- **Duration_Minutes**: Runtime in minutes.
- **Viewer_Rating**: Average viewer rating (float, 0-10 scale).
- **Number_of_Reviews**: Number of user reviews.
- **Language**: Primary language.
- **Country**: Country of origin.
- **Watched_Percentage**: Average percentage of content watched.
- **Is_Original**: Whether the content is platform-original (True/False).
- **Actors**: List of main actors.
- **Tags**: Comma-separated tags (e.g., Action,Adventure,Thriller).
- **Description**: Brief content description.

## Notebook Structure
The Jupyter Notebook (`Streaming_Content_Analysis.ipynb`) is organized into the following steps:
1. **Import Libraries**: Loads pandas, matplotlib, seaborn, wordcloud, and other dependencies.
2. **Load and Clean Data**: Handles missing values, converts `Release_Year` to Int64, and addresses outliers (e.g., unrealistic durations).
3. **Genre Distribution Analysis**: Visualizes genre frequency with a bar graph and identifies the top 3 genres (Drama: 1547, Action: 1238, Comedy: 1065).
4. **Platform Performance Analysis**: Shows content count and average ratings per platform (Netflix: 2412 titles, Disney+: 7.14 average rating).
5. **Original Content Success Analysis**: Compares originals vs. non-originals on ratings, watched percentage, and reviews.
6. **Tag Word Cloud**: Generates a word cloud for tags and lists the top 5 (Drama: 1398, Action: 1102, Comedy: 987, Thriller: 876, Adventure: 754).
7. **Interesting Fact**: Identifies high-rated but under-watched titles as potential hidden gems.
8. **Conclusion**: Summarizes key findings and actionable insights.

## Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - pandas
  - matplotlib
  - seaborn
  - wordcloud
  - numpy

## Setup Instructions
1. **Clone the Repository** (if applicable):
   ```bash
   git clone <repository-url>
   cd streaming-content-analysis
2. **Install dependencies**
   ```bash
   pip install pandas matplotlib seaborn wordcloud numpy
3. **Ensure Dataset Availability**: Place streaming_content_dataset.csv in the project directory.
4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook Streaming_Content_Analysis.ipynb
