# Good Seed Supermarket - Age Verification Model

## Project Description

Good Seed Supermarket is looking to explore if data science can help them comply with alcohol regulations by ensuring they do not sell alcohol to minors. They have asked you to evaluate this, and when you begin working, keep the following in mind:

- The stores are equipped with cameras at the checkout area, which are activated when a person is purchasing alcohol.
- Computer vision methods can be used to determine a person’s age from a photo.
- The task is to build and evaluate a model that verifies people's age.

To begin working on this task, you will be provided with a set of photos of people along with their ages.

#### Training and Evaluation

We will use a pre-trained model for this task, specifically one trained on a large image dataset called ImageNet. You can review the dataset on Kaggle:  
[ImageNet Dataset on Kaggle](https://www.kaggle.com/c/imagenet-object-localization-challenge/data).

You can find the original dataset information here:  
[ImageNet Official Website](http://www.image-net.org/).

However, we recommend using Kaggle. Remember to create a Kaggle account if needed.

Note that this dataset is not strictly about faces, so the pre-trained weights may not work perfectly for this task. However, it's still valid to use this dataset for face classification, as ImageNet contains a subset of face images. By setting the 'weights' parameter to 'imagenet', we can load pre-trained weights from the ResNet50 architecture.

### Exercises

#### Exercise 1: Model Training

1. Build and train a convolutional neural network (CNN) using the dataset with people’s photos.
2. Obtain an MAE value for the test set no higher than 8.

Your script should contain four functions:
- `load_data(path, subset)`: Loads the training and test datasets.
- `create_model(input_shape)`: Defines the model.
- `train_model(model, train_data, test_data, batch_size, epochs)`: Controls the training of the model. You should set `epochs` to 3. Training the model may take some time, so be patient.

For reference, the lowest MAE achieved on this dataset is 5.4. If you get an MAE below 7, that would be a great result!

Add the model training results (as returned by the GPU platform) to the Jupyter notebook you created during the EDA phase so everything is in one place. Then analyze the results of the model training.

### Discussion

- Can computer vision help the client in this case?
- What other practical tasks could the client solve with this model? Share your ideas.

## Conclusion

This project explores how computer vision techniques can assist in verifying the age of customers purchasing alcohol, ensuring compliance with alcohol sales regulations. The process involves data exploration, model training using pre-trained networks, and evaluating the model's performance. The goal is to assess the practical applicability of machine learning and computer vision for real-world problems in retail environments.

