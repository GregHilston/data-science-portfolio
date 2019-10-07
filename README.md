# Data Science Portfolio by Gregory Hilston

This repository is to act like a high level overview of the data science projects I've worked on. Each project's `README.md` should act as a full description of the project, but I'll provide a short description here for convenience. All of these projects are in Python. Links are provided to projects whose code can be made public.

## Kaggle Competitions

- [Talking Data Ad Tracking Fraud Detection Challenge](https://github.com/GregHilston/kaggle-talking-data-ad-tracking-fraud-detection-challenge)
  - Classification challenge on a mobile advertisement data where fraudulent clicks were the class of interest. I spent most of my time on the exploratory data analysis (EDA) and used a random forest classifier for my submission. The data set was over one hundred thirty five million rows, so I used an elastic compute cloud (ec2) instance on amazon web services (AWS) for processing.

## Visualizations

- [Meteorites](https://github.com/GregHilston/meteorites)
  - Visualized geospatial meteorite data using pandas, seaborn, matplotlib, numpy and folium.
- [It Is Wednesday My Dudes Google Trends](https://github.com/GregHilston/It-Is-Wednesday-My-Dudes-Google-Trends)
  - Investigated Google Trends data with pandas and matplotlib to prove, visually, a time series trend.

## Presentations

- Markov Chains
  - This presentation was a fun, interactive, way to explain what Markov Chains are and how they can be used to generate new sentences, given a corpus. The text of books, and scripts of television shows were used to demonstrate having a corpus, and sentences were generated against the entire corpus, as well as per character. Additionally, all Slack messages sent in the channels #general and #random were used to demonstrate generating sentences, for each coworker. Two small games were played:
    1. Was this sentence actually sent by this person, or is it generated?
    2. Given these five generated sentence, which person was this Markov Chain trained on?
- [Pandas](https://github.com/GregHilston/ds_pandas_presentation)
  - This presentation was not a lecture format, rather participants broke up into small groups and walked through a Jupyter Notebook together. The Notebook was broken up into sections, some of which were simply reading and executing lines of code to learn the basics. The last section involved twenty challenges to introduce the user with Pandas commands.
- [Word Embeddings](https://github.com/GregHilston/word_embeddings_presentation)
  - Discuss what word embeddings are and what they can be used to do. Combines a lecture format with an IPython Notebook that can be used independently by the viewers or part of the presentation.
- [Big Data Processing: Using Hadoop, Hive and Pig](https://drive.google.com/open?id=13CXGWy9SMo22tm938tRZvdPaIWbfcdSR)
  - A high level summary of what I learned during [Johns Hopkins' course 605.788 Big Data Processing Uisng Hadoop](https://ep.jhu.edu/programs-and-courses/605.788-big-data-processing-using-hadoop). Walks through the same example using Hadoop, Hive, Pig and Spark to allow the viewers to form their own opinions on the strengths and weaknesses of each project.
- [General Adversarial Networks](https://drive.google.com/open?id=1IPM8F2ArYy6ZDnD970HGRfsrirDozufn)
  - A high level summary of what General Adversarial Networks are and how they can be used. Best given to an audience with little to no data science background. Very interesting and easy to follow by someone with little to no technical or relevant technical background.

## Natural Language Processing (NLP)

[comment]: # (% ds-most-important-phrases-in-corpus-api and ds-most-important-phrases-in-corpus-drone)
- Most Important Phrases In Corpus
  - Wrote a production ready micro service based system to find N "important" sentences that would summarize a given corpus. Used TF-IDF to discover "important" sentences and page rank to sort them. An API accepted jobs and posted them to amazon web services (AWS) simple queue system (SQS), while N drones pull down jobs, process the request and POST the results back to the requester. Leveraged nltk, sklearn, numpy, flask and boto3. Was used as an opportunity to create an example project for the data science team, on using:
    - Docker
    - linting (prospector and mypy)
    - Git hooks (to run linting)
    - Continuous integration continuous deployment (CircleCi)
    - Unit tests (pytest)

[comment]: # (ds_sentiment)
- User Review Sentiment Analysis
  - Implemented a cron polling system that processes users review's sentiment using flask and Google Cloud's Language API.

[comment]: # (ds_advice_local_categories)
- Inter Company Categorization Mapping
  - Automated the mapping of data from one company's categorization to another, using gensim and glove vectors.

[comment]: # (ds_synonym_generator)
- Synonym Generator
  - Generated synonyms programmatically using nltk, spacy, gensim and glove vectors to improve smart search capabilities.

[comment]: # (ds_trl_other_businesses_categorizer)
- Business Classifier
  - Classified business data using keras, spacy, gensim, sklearn and neural networks, saving years of projected manual labor.

## Dashboard

[comment]: # (% ds_trl_dashboard, ds_us_cities)
- Data Dashboard
  - Created internal dashboard using folium and dash to generate visualizations. Allowed leadership to make data driven decisions instead of going of gut reactions.
    - An example of this would be suggesting which US cities our product could target next by accounting for population, number of businesses and other data points. Rather than just choosing by gut.

## Image Processing

[comment]: # (% ds_google_cloud_vision)
- Google Vision API Wrapper
  - Developed a wrapper for Google Cloud's Vision API to filter inappropriate user submitted images, memes and determine percentage of image used by text. Written using flask and Pillow, deployed to AWS lambda using zappa.

## Recommenders

[comment]: # (% ds_trl_recommender)
- Geolocation Item Based Recommender
  - Researched item and user based recommenders for review aggregate platform using pandas, sqlalchemy and turicreate. Ended up with basic model that accounted for user's geolocation when producing recommendations.

## Data Munging (Cleaning)

While most, if not all, of these projects have a data munging aspect, the following were specifically exclusively data munging efforts.

[comment]: # (% ds_trl_hours_regularization)
- Hours Regularization
  - Took previously unformatted, no front end validation, hours data and wrote a large amount of regex to parse the hours data into a structured format. Successfully parsed ~2.3 million pieces of data, saving the company time and money. The newly formatted data can now be used programmatically for many new features. Leveraged pandas for data processing and ray for parallelizing operations, taking execution from 1.5 hours about 15 minutes.

## Games
[comment]: # (% tic-tac-toe-modeling)
- [Decision Tree Based Tic Tac Toe Player](https://github.com/GregHilston/tic-tac-toe-modeling)
  - Created a driver to play Tic Tac Toe and challenged an opponent who placed randomly. Used the random opponent to record what a good player, me, would do. Used this data set to train a Decision Tree Classifier, and then challenged this new model to play. The model fell back on randomness when the small data set fell short. Done using pandas and scikit learn.

## Book List
- [Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems by Aurélien Géron](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291)
  - Currently going through this book, while working through all exercises, challenges and code examples.
- [The Hundred-Page Machine Learning Book](https://www.amazon.com/Hundred-Page-Machine-Learning-Book/dp/199957950X/ref=sr_1_3?crid=2DZ7SSNDR0073&keywords=100+page+machine+learning+book&qid=1567686509&s=gateway&sprefix=100+page+m%2Caps%2C187&sr=8-3)

[comment]: # (needed internally ds_adwords, ds_reports, ds_reporter)
