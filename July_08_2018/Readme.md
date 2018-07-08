## Deep Learning Rest API using Keras

### Set up your own environment (install necessary packages)

I assume you already have Keras and Flask installed on your system. If they are not please install it first.</br>
Next,</br>
```pip install flask gevent requests pillow```

Next clone the repo:

```git clone https://github.com/Praneet460/100DaysofMLCode.git```

### Start the Keras server

The Flask + Keras server can be started by running:

```python keras_server.py```

You can now access the Rest API via ```http://127.0.0.1:5000```

Request can be submitted via cURL:

```curl -X POST -F image=@dog.jpg "http://127.0.0.1:5000/predict"```</br>
```curl -X POST -F image=@cat.jpeg "http://127.0.0.1:5000/predict"```</br>
```curl -X POST -F image=@rabbit.jpg "http://127.0.0.1:5000/predict"```

Below you can see the image we wish to classify:
1. A dog, but more specifically a beagle.

![Dog](https://github.com/Praneet460/100DaysofMLCode/blob/master/July_08_2018/dog.jpg)

```{
  "predictions": [
    {
      "label": "beagle", 
      "probability": 0.9901360869407654
    }, 
    {
      "label": "Walker_hound", 
      "probability": 0.002396771451458335
    }, 
    {
      "label": "pot", 
      "probability": 0.0013951235450804234
    }, 
    {
      "label": "Brittany_spaniel", 
      "probability": 0.001283277408219874
    }, 
    {
      "label": "bluetick", 
      "probability": 0.0010894243605434895
    }
  ], 
  "success": true
} 
```

2. A cat, but more specifically an egyptian cat.

![Cat](https://github.com/Praneet460/100DaysofMLCode/blob/master/July_08_2018/cat.jpeg)


```{
  "predictions": [
    {
      "label": "Egyptian_cat",
      "probability": 0.7509434819221497
    },
    {
      "label": "tabby",
      "probability": 0.1136670634150505
    },
    {
      "label": "lynx",
      "probability": 0.042728323489427567
    },
    {
      "label": "tiger_cat",
      "probability": 0.024716876447200775
    },
    {
      "label": "Persian_cat",
      "probability": 0.018322255462408066
    }
  ],
  "success": true
}
```

3. A rabbit, but more specifically a hare.

![rabbit](https://github.com/Praneet460/100DaysofMLCode/blob/master/July_08_2018/rabbit.jpg)

```{
  "predictions": [
    {
      "label": "hare",
      "probability": 0.8665587902069092
    },
    {
      "label": "wood_rabbit",
      "probability": 0.09570298343896866
    },
    {
      "label": "Angora",
      "probability": 0.03592341020703316
    },
    {
      "label": "wallaby",
      "probability": 0.0006861469591967762
    },
    {
      "label": "hamster",
      "probability": 0.0005263470811769366
    }
  ],
  "success": true
}
```
