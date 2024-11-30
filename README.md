# YouTube-Watch-Habits-Analysis-and-Personalized-Recommendations

# Research Questions

How do viewing habits differ across various times of the day, and what content categories dominate these periods?

How can time-based analysis of YouTube watch history be used to generate personalized video and channel recommendations?

# Research Aim
The primary goal of this project is to understand your YouTube watch habits by analyzing the watch history extracted from Google Takeout. 

This includes:

Identifying time-based viewing patterns.
Categorizing content by genres, channels, or themes.
Providing personalized recommendations based on your habits and preferences.
Visualizing the results to make insights easily interpretable.

# Data Source

Google Takeout: Export your YouTube watch history as JSON files.
Path in the Takeout archive: YouTube and YouTube Music/History/watch-history.json.

Data fields include:

title: Video title.
subtitles: Channel name.
time: Timestamp of when the video was watched.
details: Metadata about the device or context (if available).

# Steps to Execute the Project
1. Data Collection
   
   
Export your YouTube data from Google Takeout.
Locate the file watch-history.json in the archive.
Load the data into a Python script for preprocessing.

2. Data Preprocessing
   
Clean the Data:

Remove duplicate entries.
Parse timestamps into usable formats (e.g., date, hour, weekday).
Extract Key Features:

Video Title: Identify unique or recurring titles.
Channel Name: Analyze the most-watched channels.
Timestamp: Group by time of day (morning, afternoon, evening, night).

3. Explanatory and Exploratory Data Analysis


Explanatory Goals:

Understand Time-Based Viewing Habits:
Analyze the distribution of watch times across periods (morning, afternoon, evening, night).
Identify Content Preferences:
Find your most-watched channels and content types.
Detect Patterns in Content Themes:
Categorize videos by themes (e.g., comedy, educational) to understand preferences.

Exploratory Questions:

What times of the day do you watch the most videos?
Which channels dominate your watch history?
Are there trends in the types of videos watched during specific periods?

4. Visualizations
   
Visualization Goals:

Heatmap of Viewing Activity:
Display hours of the day vs. number of videos watched.
Bar Chart of Most-Watched Channels:
Highlight your top 10 most-watched channels.
Pie Chart of Content Themes:
Show the percentage distribution of content themes (if categories are defined).
Time Series Analysis:
Analyze weekly or monthly viewing trends.

5. Recommendations
   
How Recommendations Work:

Pattern Matching:

Identify recurring shows, themes, or channels.
Example: If you watch sitcoms like Yalan Dünya at night, prioritize comedy recommendations for nighttime.
Fetch Related Content:

Use the YouTube Data API or pre-built tags to suggest similar videos.
Example: Recommend other Turkish sitcoms or user-created playlists.
Dynamic Playlists:

Curate playlists based on your preferences:

Morning Playlist: Educational or motivational videos.
Nighttime Playlist: Relaxing or lighthearted content.
