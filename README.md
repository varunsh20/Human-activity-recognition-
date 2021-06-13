# Human-activity-recognition

This is a kaggle project. Here is the link to the kaggle dataset:https://www.kaggle.com/uciml/human-activity-recognition-with-smartphones

The Human Activity Recognition database was built from the recordings of 30 study participants performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors. The objective is to classify activities into one of the six activities performed.

The six activities includes 'Standing', 'Sitting', 'Laying', 'Walking', 'Walking_downstairs', 'Walking_upstairs'.

A multi layer perceptron network was trained. Here is the structure of the model

model = models.Sequential()

model.add(Dense(64,activation='relu',input_dim=X_train.shape[1]))
model.add(Dropout(0.25))
model.add(Dense(128,activation='relu'))
model.add(Dense(64,activation='relu'))
model.add(Dense(32,activation='relu'))
model.add(Dropout(0.25))
model.add(Dense(10,activation='relu'))
model.add(Dense(6,activation='softmax'))

This model was able to produce 93% accurate results.

## Confusion matrix

![ha1](https://user-images.githubusercontent.com/62187533/121818537-6e789b00-cca5-11eb-82de-a45cb0909618.png)

