# YouTube-Watch-Habits-Analysis-and-Personalized-Recommendations

Overview
This project analyzes your YouTube watch habits with a focus on time of day and content preferences. It identifies patterns in your viewing history, such as frequently watched videos or channels during specific hours, and provides personalized recommendations for channels and videos.

For example, if you tend to watch sitcoms like Yalan Dünya or Avrupa Yakası before bed, the system detects this habit and recommends similar videos or channels for your nighttime routine.

Features
Time-Based Analysis:

Detect when you watch the most (morning, afternoon, evening, or night).
Visualize watch activity with heatmaps and bar charts.
Content Categorization:

Identify the types of videos you watch during different time periods (e.g., educational in the morning, relaxing shows at night).
Categorize videos by genres, channels, or themes.
Personalized Recommendations:

Suggest channels and videos tailored to your viewing habits.
Generate time-specific playlists (e.g., morning motivation, nighttime relaxation).
Channel Insights:

Highlight your most-watched channels.
Recommend similar channels or underexplored creators in your preferred genres.
Dynamic Playlists:

Create curated playlists based on your viewing patterns and preferences.
How the Project Works
1. Data Collection
Fetch watch history using the YouTube Data API, including:
Video titles.
Timestamps of when videos were watched.
Channels and categories.
2. Data Analysis
Extract patterns from watch history:
Time Analysis: Group videos by the hour and day of the week.
Content Categorization: Use video metadata to identify themes or genres.
Identify recurring habits, such as:
Watching sitcoms before bed.
Viewing educational content during the day.
3. Recommendations
Fetch similar videos using the YouTube API:
Related videos based on titles, tags, and categories.
Channels that produce similar content to your favorites.
Generate playlists tailored to specific times or preferences.
4. Visualization
Heatmaps for hourly watch activity.
Bar charts for content categories by time of day.
Pie charts showing most-watched channels and genres.
Technical Details
APIs Used
YouTube Data API:
GET /videos: Fetch video details and metadata.
GET /playlistItems: Retrieve watch history.
GET /search: Find related videos.
Optional APIs:
TMDb API (if extending to movies/TV shows).
OpenWeatherMap API (if integrating weather).
Tools and Libraries
Data Handling:
Pandas: Data analysis and grouping.
NumPy: Time-based calculations.
Visualization:
Matplotlib: Heatmaps and bar charts.
Plotly: Interactive visualizations.
Recommendation System:
scikit-learn: Clustering for similar videos.
google-api-python-client: YouTube API integration.
