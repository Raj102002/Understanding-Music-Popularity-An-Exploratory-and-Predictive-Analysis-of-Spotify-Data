Spotify Songs Dataset: Full Insights Summary
# Understanding-Music-Popularity-An-Exploratory-and-Predictive-Analysis-of-Spotify-Data
This project explores the key factors that drive the popularity of songs on Spotify using a comprehensive dataset of top tracks across 73 countries, updated daily. By combining exploratory data analysis, audio feature extraction, and machine learning models.
1. Average Popularity by Country
Insight:

Top countries with highest average popularity are:
🇳🇿 New Zealand, 🇦🇺 Australia, 🇨🇦 Canada, 🇬🇧 UK, 🇺🇸 US.
These countries are trend adopters or may have stronger streaming cultures.

📈 2. Popularity Trends Over Time (Top 3 Songs)
Songs Analyzed:
Die With A Smile, BIRDS OF A FEATHER, Espresso

Insights:
Songs sustain high popularity scores consistently.
Sharp dips to 0 are likely missing data points or days when the song didn’t chart, not actual unpopularity.
"Die With A Smile" maintains the most stable top performance.

3. Explicit vs Non-Explicit Songs
Insight:

Explicit songs (True) have a slightly higher median popularity than non-explicit ones.
Implication: Genres like rap, trap, edgy pop, which often use explicit lyrics, might drive engagement.
However, the popularity distribution overlaps significantly, suggesting non-explicit songs can also be major hits.

4. Correlation of Audio Features with Popularity
Popularity Correlations:
Feature	Correlation with Popularity
Danceability	-0.046
Energy	-0.016
Valence	-0.020
Tempo	-0.027
Speechiness	-0.15
Loudness	+0.026
Instrumentalness	+0.033
Acousticness	-0.072
Insights:
Most features have very weak correlation with popularity — no single audio trait guarantees success.
Speechiness has a negative correlation: songs that are very "talky" (e.g., spoken word) tend to be less popular.
Loudness and instrumentalness show tiny positive correlation, suggesting a slight edge in popularity for louder or instrumental-rich tracks.
Takeaway: Musical style alone doesn’t predict popularity — external factors like artist, marketing, trend virality, and audience matter more.

Combined Takeaways
Category	Key Insight
Country Trends	Top streaming countries (NZ, AU, CA) are consistently aligned with global trends.
Time Series	Hit songs maintain strong performance across time with occasional dropouts.
Explicit Content	Explicit songs may slightly edge out in popularity, but it's not a rule.
Audio Features	Popularity is not strongly tied to features like danceability, energy, etc.
Weak Correlation	No strong predictor → success is likely multi-factorial and cultural.

Machine learning models:

1. Logistic Regression (Binary Hit Classification)
Transformed song popularity into binary classification (hit or not).
Model Results:
Accuracy: 60%
Precision: 0.61 (class 0), 0.58 (class 1)
F1-score: ~0.60
Good baseline model but lacked nuance in complex audio relationships.

2. Random Forest Classifier
Significantly better performance than Logistic Regression:
Accuracy: 89%
Precision: 0.88 & 0.91
F1-score: 0.89
Top features for hit prediction: energy, danceability, loudness, and speechiness.

Insights:
Explicit songs tend to receive more attention globally.
Songs with high energy and danceability are more likely to become hits.
Audio loudness and speech-like elements contribute positively to popularity.
Random Forest outperforms Logistic Regression in predicting whether a song will be a hit.
