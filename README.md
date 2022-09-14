
### New ESRB Category following the CRISP-DM method

Helps demonstrate a need for a new categorization for video game ratings through machine learning techniques
Motivation: We want to see if Teen is too much of a catchall for most game ratings and if so what could elucidate a new categorization


## Run the project

This project runs on Python 3.7.12  once you confirm the settings you can start on this project.

Clone the project

```bash
  git clone https://github.com/aadejare/new_esrb_rating
```

Go to the project directory

```bash
  cd new_esrb_rating
```

Install dependencies

```bash
numpy = 1.21.6
pandas = 1.3.5
sklearn = 1.0.2
xgboost = 1.6.1
```

Grab data from the data source and run from Jupyter Notebook You can grab a method of running a Jupyter Notebook from Anaconda https://www.anaconda.com/
Running the project, you will notice that there are some plots as well as extra variables to try out.  I encourage you to play with the "esrb_rating"
category to see if new labels can be generated as well as potentially predicting a rating.
The best machine learning technqiue used was xgboost, but I would not be surprised if it performed well becasue it works with sparse data.


## Data source

The Data source comes from Kaggle [Video Games Rating By 'ESRB dataset'](https://www.kaggle.com/datasets/imohtn/video-games-rating-by-esr)

Download the files and replace the file paths with where the files are located on your machine.

The data sources are the following
```
Video_games_esrb_rating.csv: Traninig dataset containing records that have the ratings and the descriptions that merrit the rating
test_esrb.csv: New dataset to evaluate model  
```
## Deployment

To deploy this project you need the following package

```bash
numpy = 1.21.6
pandas = 1.3.5
sklearn = 1.0.2
xgboost = 1.6.1
```


## Results

Here were the Results
KBQ1: XGBoost had the highest accuracy and F1 score for teen prediction
KBQ2: Using Kmeans clustering, Teens label had the least clarity on cluster location and subsequently had variables that were hard to decern for a perfect laebl.
KBQ3: Action titles seemed to be the candidates for a new label with violence, language, and use of alcohol being some of the most frequent categories that provided contenxt as to whether to produce a new label or not.

There's more but you should play around with it and discover more through the notebook.
## Acknowledgements

 - [Udacity](www.udacity.com)
 - [Kaggle](www.kaggle.com)
 - [Entertainment Software Rating Board ](www.esrb.com)


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Authors

- [@aadejare](https://www.github.com/aadejare)

