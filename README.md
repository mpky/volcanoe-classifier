# Volcanoes on Venus Image Classifier

#### Project Goal

Train several supervised learning models (Random Forest, SVM, XGBoost, Logistic Regression, CNN) to recognize if a given image of the planet Venus has a volcano in it or not and compare model performance.

#### Motivation

Manually labeling images such as this for binary classification is a tedious process; a high-performing image classifier can speed that up. Because of how regular the appearance of the volcano is in most of the photos, I also wanted to determine if a more simple model could perform as well as a more powerful, but slower Convolutional Neural Network.

#### Dataset

The dataset contains 9,734 images of the surface of Venus taken by NASA's Magellan spacecraft. The images were labeled and uploaded to Kaggle [here](https://www.kaggle.com/fmena14/volcanoesvenus).

#### Implementation and Training

I trained and then tested Random Forest, Gradient Boosting, XGBoost, Ridge Regression, Lasso Regression, Logistic Regression, and Support Vector Machines. I then performed some PCA on the data to see if that would improve the performance for any of these baseline models. Lastly, I trained several Convolutional Neural Networks to compare performance with the faster baseline models.

#### Results

Several baseline models such as Ridge and Lasso Regression were able to perform quite well, but the best CNN was the highest performer by some margin. Ridge Regression had an accuracy score of 0.9268 on the test data; Lasso had an accuracy of 0.9283, which makes sense given how wide the image dataset is. The CNN had an accuracy score of 0.9814 on the testing data.

#### Other Notes

- PCA did not help the baseline models.
- Most baseline models performed quite well without much parameter-tuning.

##### Strongest Predictions from the Best-performing Neural Network

<img width="883" alt="Untitled" src="https://user-images.githubusercontent.com/31871105/58878041-575b4780-86a0-11e9-9fc5-7c7213f79dae.png">
