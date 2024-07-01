# CNN Model ~ Vehicle Type Prediction

I used a personal dataset to train our model and put it in the 'VehicleImages' folder. It has around 25k images consisting of buses, cars, and motorcycles. 

Successfully achieved a <b>96% accuracy</b>.

## Impact
The CNN model I have built has the potential to solve everyday road issues. With the ability to predict between types of vehicles, it can be made simpler to avoid congestion in certain parts of a location. For
example, some roads are clearly stated for only buses to drive on hence allowing them to be on their scheduled time. However, sometimes to skip the traffic often cars and motorcycles take such restricted
roads. Utilizing the model, we can fix this problem by stopping other vehicle types from entering or imposing fines as a measurement to prevent unnecessary traffic congestion.

<hr>

Imported modules:
<li>Pandas</li>
<li>Numpy</li>
<li>os</li>
<li>Tensorflow</li>
<li>Matplotlib</li>

<br>

Firstly, I converted our dataset into a DataFrame using pandas, with 2 columns: Images and Labels. I had to store the images as their relative paths and gave them their respective Label. The next step was to split the dataset into training and testing with an 80:20 split. After splitting our data, I performed augmentation and pre-processing using ImageDataGenerator from the TensorFlow library.

Time to build our model! The model consists of 3 2D Convolution layers, 3 2D Max Pooling layers, Flatten Layer, Dropout Layer, and Dense layers. Moving forward, we define our optimizer, loss, and metrics. This way we bring our model to completion.

# Evaluation
The following graphs show the accuracy and loss throughout the 20 epochs.

![image](https://github.com/HarshaBeth/CNN-Vehicle-Prediction/assets/92636321/b47a6db6-93b9-4697-a0aa-e29a0e459bc6)
![image](https://github.com/HarshaBeth/CNN-Vehicle-Prediction/assets/92636321/21f590b9-dcc6-485e-8e77-04b0c7d042c7)

# Prediction
With these amazing results, it was time to test the model. So, I selected random images of cars, buses, and motorcycles from the internet completely out of our dataset to ensure there is no bias.
The prediction outcomes are as great as expected!

![image](https://github.com/HarshaBeth/CNN-Vehicle-Prediction/assets/92636321/f2ee1be7-7568-49f3-b579-e97f72e07db0)
![image](https://github.com/HarshaBeth/CNN-Vehicle-Prediction/assets/92636321/68ee7679-9317-4617-a087-d651da4345cc)
![image](https://github.com/HarshaBeth/CNN-Vehicle-Prediction/assets/92636321/e927bb9b-d01f-4df0-9a3f-f80a7a338073)








