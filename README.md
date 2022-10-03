# Machine_Learning_Algorithmic_Trading_Bot

This model uses machine learning classification methods through scikit learn to predict algorithmic trading strategies.

---

## Technologies

This analysis uses python Python and the following libraries:
* [Pandas](https://pandas.pydata.org/) - Provides data manipulation and visualization necessary to conduct this analysis
* [NumPy](https://numpy.org/doc/stable/user/index.html#user) - Provides scientific computing
* [Pathlib](https://docs.python.org/3/library/pathlib.html) - Provides the path to a CSV database
* [scikit-learn](https://scikit-learn.org/stable/user_guide.html) - Machine learning tools written in Python
---

## Installation Guide

1. Download [Anaconda](https://www.anaconda.com/products/distribution) to your computer. 

2. Clone the repo to your local machine

3. Run the following command in your terminal or gitbash:
```python
pip install -r requirements.txt
```

---

## Usage

These models are free to use by any interested persons.

---

## Model Analysis

The original SVM model had an accuracy score of 49% and consistently performed better than the actual returns.

![Best_Strategy_Returns](https://github.com/rrmangum/Machine_Learning_Algorithmic_Trading/blob/main/Images/Best_Strategy_Return.png?raw=true)

Adjusting the size of the training dataset to only include data from May 2018 and forward 
turned the strategy from profitable, to an overall loss. However, the accuracy of the model increased from 49% to 55%. While this model is technically more accurate at prediciting the outcomes than the original, this strategy overall returns less than the original model.

An alternative model uses the original dataset, but alters the short SMA window to 20 and the model increased in accuracy from 49% to 51%, however this model also flipped the strategy from profitable to unprofitable.

Finally, a third model using Logistic Regression, also failed to produce strategy returns greater than the baseline model.

![LR_Model_Returns](https://github.com/rrmangum/Machine_Learning_Algorithmic_Trading/blob/main/Images/LR_Model_Strategy_Return.png?raw=true)

The original model produced the best strategy returns from the tested models.

IMAGE

---

## Contributors

Ryan Mangum - [LinkedIn](https://www.linkedin.com/in/ryanrmangum/) | rrmangum@gmail.com

---

## License

[MIT License](https://choosealicense.com/licenses/mit/)

Copyright (c) [2022] [Ryan Mangum]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.