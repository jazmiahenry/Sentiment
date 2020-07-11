# Sentiment
The goal of this modeling challenge is to show my ability to make complex models to make sentiment analysis using the data provided. Below is not only code used to acheive those ends, but also information on how these models can be improved. As a computer scientist, I care not only able writing easily digestable and readable code, but also acknowledging possible places of improvement. I strive to always grow as a scientist and engineer. Thank you.

# Accuracy Scores: 
- Accuracy for C=0.01: 0.9565142660708147
- Accuracy for C=0.05: 0.9565142660708147
- Accuracy for C=0.25: 0.9569439669989687
- Accuracy for C=0.5: 0.9582330697834307
- Accuracy for C=1: 0.9621863183224476


## Data transformation Improvement
    Data could be more appropriately engineered using PostgreSQL to:
        1. Avoid duplicate data across dataframes while merging
        2. Joining Dataframes by simular columns (ie joining date_posted and date_time_collected)
        3. Using SQLite to process SQL table in Jupyter notebook and transform into Dataframe using Pandas

## Improvements to the Sentiment Analysis
    Translate all captions into English.
        A. Import LangDetect and Googletrans packages 
        B. Turn df.caption into a dataframe
        C. Identify non-English words and translate into English using Googletrans
        D. Use caption dataframe for sentiment analysis preproccessing 

