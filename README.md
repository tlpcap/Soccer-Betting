# Soccer-Betting

Beta* 

A project to pit predictions to reality using machine learning; 

A repo to predict soccer scores from Historical train data and timetable & test data. 

We use Scikit-Learn's RandomForestRegressor to predict soccer scores based on historical data and betting odds.
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html

By data enthusiasts for betting enthusiasts.

Steps to follow:

	1. Run Step-1-To download Historical Data (1993-2019).py to download historical data as available on http://football-data.co.uk/ on major European Leagues and save it into one consolidated .csv, which will be used as training data
	2. Run Step-2-Download Updated Data and concat with Historical Data.py to update training data to reflect the latest results
	3. Run Step-3-BET365 odds scraper_raw.py to download https://www.bet365.com odds for all respective leagues. This is required to predict outcomes. We use https://github.com/S1M0N38/soccerapi to scrape betting odds.
	4. Run Step-4-Normalizing Odds.py to normalize team names and split the odds dictionary list into a flat consumable format, which will be used as testing data
	5. Run Step-5-Predicting.py to predict outcomes present in testing data
