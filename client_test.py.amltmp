import requests
import numpy as np
import random
from tensorflow.keras.datasets import mnist
import matplotlib.pyplot as plt

(_, _), (x_test, y_test) = mnist.load_data()

#picks a random image from test data
idx = random.randint(0, 312)
image = x_test[idx]
print(image.shape)
label = y_test[idx]
print("Actual label:", label)

url = 'http://127.0.0.1:5000/predict'
data = {
    'input': image.tolist()
}

response = requests.post(url, json=data)
print(response.json())