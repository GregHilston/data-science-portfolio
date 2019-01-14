# Data Science Portfolio by Gregory Hilston

This repository is to act like a high level overview of the data science projects I've worked on. Each project's `README.md` should act as a full description of the project, but I'll provide a short description here for convenience. All of these projects are in Python. Links are provided to projets whose code can be made public.

## Kaggle Competitions

- [Talking Data Ad Tracking Fraud Detection Challenge](https://github.com/GregHilston/kaggle-talking-data-ad-tracking-fraud-detection-challenge)
  - Classification challenge on a mobile advertisement data where fradulant clicks were the class of interest. I spent most of my time on the exploratory data analysis (EDA) and used a random forest classifier for my submission. The data set was over one hundred thirty five million rows, so I used an elastic comute cloud (ec2) instance on amazon web services (AWS) for processing.

## Visualizations

- [Meteorites](https://github.com/GregHilston/meteorites)
  - Visualized geospatial meteorite data using pandas, seaborn, matplotlib, numpy and folium.
- [It Is Wednesday My Dudes Google Trends](https://github.com/GregHilston/It-Is-Wednesday-My-Dudes-Google-Trends)
  - Investigated Google Trends data with pandas and matplotlib to prove, visually, a time series trend.

## Presentations

- [Word Embeddings](https://github.com/GregHilston/word_embeddings_presentation)
  - Discuss what word embeddings are and what they can be used to do. Combines a lecture format with an IPython Notebook that can be used independently by the viewers or part of the presentation.
- [Big Data Processing: Using Hadoop, Hive and Pig](https://drive.google.com/open?id=13CXGWy9SMo22tm938tRZvdPaIWbfcdSR)
  - A high level summary of what I learned during [Johns Hopkins' course 605.788 Big Data Processing Uisng Hadoop](https://ep.jhu.edu/programs-and-courses/605.788-big-data-processing-using-hadoop). Walks through the same example using Hadoop, Hive, Pig and Spark to allow the viewers to form their own opinions on the strengths and weaknesses of each project.
- [General Adversarial Networks](https://drive.google.com/open?id=1IPM8F2ArYy6ZDnD970HGRfsrirDozufn)
  - A high level summary of what General Adversarial Networks are and how they can be used. Best given to an audience with little to no data science background. Very interesting and easy to follow by someone with little to no techninal or relevant technical background.

## Natural Language Processing (NLP)

[comment]: # (ds_advice_local_categories)
- Inter Company Categorization Mapping
  - Automated the mapping of data from one company's categorization to another, using gensim and glove vectors.

[comment]: # (ds_synonym_generator)
- Synonym Generator
  - Generated synonyms programmatically using nltk, spacy, gensim and glove vectors to improve smart search capabilities.

[comment]: # (ds_trl_other_businesses_categorizer)
- Business Classifier
  - Classified business data using keras, spacy, gensim, sklearn and neural networks, saving years of projected manual labor.

[comment]: # (ds_sentiment)
- User Review Sentiment Analysis
  - Implemented a cron polling system that processes users review's sentiment using flask and Google Cloud's Language API.

## Dashboard

[comment]: # (% ds_trl_dashboard, ds_us_cities)
- Data Dashboard
  - Created internal dashboard using folium and dash to generate visualizations. Allowed leadership to make data driven decisions instead of going of gut reactions.

## Image Processing

[comment]: # (% ds_google_cloud_vision)
- Google Vision API Wrapper
  - Developed a wrapper for Google Cloud's Vision API to filter inappropriate user submitted images, memes and determine percentage of image used by text. Written using flask and Pillow, deployed to AWS lambda using zappa.

## Recommenders

[comment]: # (% ds_trl_recommender)
- Geolocation Item Based Recommender
  - Researched item and user based recommenders for review aggregate platform using pandas, sqlalchemy and turicreate. Ended up with basic model that accounted for user's geolocation when producing recommendations.

## Book List
- [Hands-On Machine Learning with Scikit-Learn and TensorFlow: Concepts, Tools, and Techniques to Build Intelligent Systems by Aurélien Géron](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291)
  - Currently going through this book, while working through all exercises, challenges and code examples.

[comment]: # (needed internally ds_adwords, ds_reports, ds_reporter)