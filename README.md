# Facial Recognition with Python ML

**This repository contains the Python code for both classification algorithms and neural networks, *as a Jupyter Notebook file*, and facial data for classifying faces using machine learning.**

## In this Repository:
- Jupyter Notebook file using **ML Classification Algorithms**
- Jupyter Notebook file using **ML Neural Networks**
- CSV containing **facial data**

The facial data is in the form of a CSV and contains facial data such as the **distance between the cheeks, eyes, corners of the mouth, nose and mouth, and the classification for each data instance, *a number.***

Feel free to go ahead and substitute the facial data in the CSV with some of your own data and parameters. **The facial data was obtained using Firebase's ML Kit to get the positions of facial features and calculating the distance between them.**

## **Classification Algorithms** used include:
- **K Nearest Neighbors (KNN)**
- **Support Vector Classifier (SVC)**
- **Decision Tree (DT)**
- **Random Forests**
- **Gaussian Naive Bayes (GNB)**
- **Logistic Regression (LR)**

## Other Features:
- **Grid Search Algorithm:**
- **Hyperparameter Optimization:**
- **Graphs, Tables, and Charts**

---
## New to Machine Learning?
Whether you're **new to ML**, or already know a thing or two, I have made a very detailed **GitHub Wiki** that you can check out to understand what Machine Learning is, how it works, and how it is implemented.

It contains detailed notes, diagrams, pictures, and code with comments.

---
## Usage
To use the code, simply download either one of the Jupyter Notebook files, or both. *One contains the code for using [classification algorithms] for facial recognition while the other uses neural networks.

For your convenience, **a CSV containing sample facial data has also been attached,** that way, you can download the CSV as well and try the code for yourself. 

**Please ensure the following are true:**
- You have the required Python modules installed, such as **`pandas`, `sklearn`, and more**. *If not*:
   - *it is recommended that you use the [pip package manager](https://pip.pypa.io/en/stable/installing/) to download the required modules.*
   - ***OR*** *Use [Google Colab](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true) which is free, online, and does not require you to download modules.*
- The CSV of facial data is in the **same directory**, at the **same level** as the Jupyter Notebook file.

## Customization
As mentioned above, the facial data in the CSV was obtained using Firebase's ML Kit. However, if you do not wish to use that to get your own set of facial data, then you can check out [**this site**](http://www.face-rec.org/databases/) which contains a list of different facial data sets that are available.

Once you get your own CSV of data, then you have to tweak the code so that it knows how many features you are using. This can be done by changing the line

    X = data.iloc[:,:4]
**TO:**

    #num is the number of features you have, excluding the class/name
    X = data.iloc[:,:num]
    
The rest of the modifications are rather straightforward because the code has comments.

**You can also make modifications to the accuracy/output of the program by changing the hyperparameters of the Classification Algorithm and the Neural Networks.**
Fortunately, I have also included detailed comments on what each of the hyperparameters are and you can also check out the **ML Wiki** that I have made.

## Additional Note
Please take into consideration that the Neural Network Facial Recognition File is **very intensive and requires a lot of resources when running. Additionally, it takes a while to run.**

You can try to lessen this by reducing the epoch number *(# of iterations)* or changing some of the other hyperparameters, but this may result in a tradeoff with accuracy.

