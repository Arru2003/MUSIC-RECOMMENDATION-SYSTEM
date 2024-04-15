
# Music Recommendation System

This Python script implements a music recommendation system using various techniques such as popularity-based recommendation and item similarity recommendation. The system utilizes a dataset containing user-song interaction data and song metadata.

## Dataset Information
The dataset consists of two files:
- **triplets_file**: Contains user_id, song_id, and the number of times a song was listened to.
- **metadata_file**: Contains song_id, title, release, artist_name, and year information.

The dataset comprises a mix of songs from various websites with user ratings based on their listening experience.

## Recommendation Systems

### 1. Popularity-Based Recommendation
- Popularity-based recommendation suggests songs based on their overall popularity among users.
- It recommends songs that are most popular or trending.

### 2. Item Similarity Recommendation
- Item similarity recommendation suggests songs similar to those a user has already listened to.
- It analyzes user-song interaction data to identify similar songs and recommend them to users.

### Types of Recommendation Systems:
- **Content-Based**: Utilizes keywords and attributes assigned to songs to match them with a user's profile.
- **Collaborative**: Filters out items based on reactions by similar users and creates a ranked list of suggestions.
- **Popularity**: Recommends popular or trending songs among users.

## Usage
1. **Import Libraries**: Import necessary libraries such as pandas and numpy.
2. **Change Directory**: Set the directory to the location of the custom recommendation module.
3. **Load the Data**: Load the user-song interaction data (`triplets_file`) and song metadata (`song_data`).
4. **Combine Dataframes**: Merge the two dataframes based on the song_id column and remove any duplicate song_ids.
5. **Data Preparation**: Create new features, such as combining title and artist name, and calculate song popularity.
6. **Popularity-Based Recommendation**:
   - Import the popularity recommender model.
   - Create the popularity recommender object and generate recommendations based on user_id.
7. **Item Similarity Recommendation**:
   - Import the item similarity recommender model.
   - Create the item similarity recommender object and generate recommendations based on user_id or song name.
   
## Example
Here's how you can use the script:
```python
python music_recommendation.py
```
Follow the instructions to generate recommendations based on popularity or item similarity for specific users or songs.

## Note
- This script provides a basic implementation of music recommendation systems. For more advanced systems, consider incorporating collaborative filtering, hybrid approaches, or neural network-based models.
