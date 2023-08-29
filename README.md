
![Drives Car Price](./images/readme_hero.jpeg)


# What Drives the Price of a Car?

This repo is a data modeling exercise based a dataset initially provided by Kaggle. While the original dataset provided information on 3 million used cars, the initial dataset used for this exercise was reduced to 426K samples to improve the performance of processing. The purpose of this exercise was to develop a model that could predict the price of a car given some subset of the other features available.

The result of this exercise was the proposal for two separate models, one that focuses on the all of the car models available as a relative predictor of price, and a second set of models built for each car model that provide a more accurate predictor of price based on the other features of the car.

## Installation

### Dependencies:
```yml
- Python: 3.11.3
- Anaconda: 2.4.0
- Jupyter Notebook: 6.5.4
- Matplotlib: 3.7.1
- Seaborn: 0.12.2
- Pandas: 1.5.3
- Numpy: 1.24.3
- Scikit-Learn: 1.2.2
```

The easiest way to install Anaconda is from the [online download source](https://www.anaconda.com/download). See the [installation page](https://docs.anaconda.com/free/anaconda/install/index.html) for more details on installation process. After downloading open Anaconda Navigator to download Jupyter Notebook

Additional dependencies can be installed from the command line using Conda:

```bash
  conda install -c matplotlib seaborn pandas numpy scikit-learn
```

After installing dependencies, run a new Jupyter Notebook instance from root of project:

```bash
  jupyter notebook
```

## Lessons Learned

Finding are summarized in the  [Final Report](./prompt_II.ipynb#Final-Report), but can roughly be summarized as follows:

The primary driver of car price appears to be based on the model of the car, with regression models built that included models as one of the features consistently having variou car models as the most heavily weighed factors for price.

Looking beyond the car model feature, it was discovered that the next most significant feature in regards to predicting price was heavily dependent on the car model in question, though year was was most commonly one of the most important predictors of price amongst all car models. As such, building a separate regression model for each car model is highly recommended if a higher degree of prediction accuracy is desired.


## Authors

[@zaldabus](https://github.com/zaldabus)


## License

[MIT License](https://choosealicense.com/licenses/mit/)