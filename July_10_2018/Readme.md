## Day 5: July 10, 2018

1. Build up a Deep learning model for classifing MNIST Dataset using Keras.
2. Tried different model and predict the accuracy:

| Model         | Testing Accuracy (%) | 
| ------------- |:----------------:    | 
| Basic Model   | 11.35                | 
| He Normal     | 75.52                | 
| Relu          | 92.88                | 
| Adam          | 92.59                | 
| Adam & Relu   | 93.85                | 
| Batchnorm     | 95.46                |
| Batchnorm & Relu | 94.71                |
| Dropout       | 11.35                |
| Ensemble      | 27.93                |

3. Most methods improve the model training & test performance. That's why we will use them all together.
4. After applying all the models together we get the accuracy near to <b>98%</b>. [Look Here](https://github.com/Praneet460/100DaysofMLCode/blob/master/July_10_2018/Final_Model.ipynb)
