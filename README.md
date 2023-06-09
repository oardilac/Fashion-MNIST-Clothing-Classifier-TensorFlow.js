# Fashion MNIST Classifier Using TensorFlow and Keras

This Jupyter Notebook demonstrates how to train a neural network using the `fashion_mnist` dataset. The model is built and trained using TensorFlow and Keras. After training, the model is evaluated, predictions are made, and the model is then saved for use in a web browser with TensorFlow.js.

## Requirements

Before you can run this notebook, you will need to have the following libraries installed:

* tensorflow
* tensorflow_datasets
* tensorflowjs

If you do not have these installed, you can install them by running this command in your notebook:

```
!pip install tensorflow tensorflow_datasets tensorflowjs
```

## How to Use

1. **Loading the Dataset**

We are using the `fashion_mnist` dataset, which contains 70,000 grayscale images of 10 categories of clothing. The dataset is already split into a training and a test set.

2. **Preprocessing the Data**

The pixel values of the images are normalized from the range 0 to 255 to the range 0 to 1. The data is then displayed for a visual inspection.

3. **Building the Model**

The model is a simple feedforward neural network. It is composed of several layers including Flatten, Dense, BatchNormalization, and Dropout layers.

4. **Compiling the Model**

The model is compiled using the Adam optimizer and the sparse categorical crossentropy loss function.

5. **Training the Model**

The model is trained for 10 epochs. Early stopping and model checkpoint callbacks are utilized.

6. **Evaluating the Model**

The loss value is plotted over time, and then the model is evaluated using the test dataset. Images from the test set are used to make predictions.

7. **Saving the Model**

Finally, the model is saved in the h5 format and then converted to the TensorFlow.js format. This model can now be loaded in a web browser using TensorFlow.js.

## Execution

You can run the entire notebook by clicking `Kernel -> Restart & Run All` in the menu. Alternatively, you can run each cell individually by clicking on a cell and then pressing `Shift+Enter`.

## Note

If you encounter any problems while running this notebook, please make sure that your environment meets the requirements. If the problem persists, feel free to open an issue.