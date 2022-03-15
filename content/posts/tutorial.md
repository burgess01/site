+++
title = "Tutorial"
image = "/images/post/post-3.jpg"
author = "Katie Burgess"
date = 2022-03-14T05:00:00Z
description = "This is meta description"
categories = ["Development Tool"]
type = "post"

+++

### Table of Contents:
- About
- Features
- Obtaining the resource
- Setup
- Execution
- Helpful Resources
- Conclusion

### About

Describe the software resource and explain its relevance to your topic. Please include the link to the software resource.

	- TensorFlow, which can be found at https://www.tensorflow.org/ , is a highly documented open source platform that can be used for machine learning. TensorFlow contains a wide variety of tools, libraries, etc., all with many articles documenting the way to use them. For machine learning, we will be focusing mainly on the library that can be downloaded in order to make implementing deep learning AI's much easier. 
	- In this tutorial, I will be going over the main features of TensorFlow, as well as how to download it and use it on your computer. I will also go over a basic machine learning example as discussed on the TensorFlow website.

---

### Features

Outline the main features of the software. Why is this software necessary for your work?

	- This software's main feature is giving the user many functions to help you build different machine learning models much easier. This software is necessary for my work because I am new to machine learning, and so this library will make the process of learning how it works a lot easier. I will need to build a complicated AI model, and so having the assistance of a library like this will shift the work for me from learning how to code these models and then figuring out how to implement mine to learning TensorFlow and then using it to implement my model, which will be a lot faster overall.

---

### Obtaining the resource

Where do you find this software resource? Is it an open source project? an online tool? How do you install it? Are there any libraries that are also necessary to install?

	- You can find TensorFlow on their website. They are a very popular programming resource and tool for machine learning. As stated before, Tensor flow is an open source software. You can download TensorFlow using pip. In order to install TensorFlow, you need the following software versions:
		- Python 3.7 or later
		- Ubuntu 16.04 or later, Windows 7 or later, or macOS 10.12.6 or later
		- pip version 19.0 or later, or version 20.3 or later for macOS
	- There are no other necessary downloads in order to use TensorFlow besides the softwares discussed above.

---

### Setup

Include steps of all necessary steps to get the software to run (for example, installations). Include the commands to run if necessary.

	- You can install TensorFlow onto your computer using pip installations. In order to install, you can use the following commands:

		``` 
		# make sure pip is upgraded to the most current version
		pip install --upgrade pip
		# install tensorflow through pip
		pip install tensorflow
		```

	- You can also install TensorFlow into a docker container to avoid using space using the following commands: 

		```
		# Download latest stable image
		docker pull tensorflow/tensorflow:latest
		# open though Jupyter server
 		docker run -it -p 8888:8888 tensorflow/tensorflow:latest-jupyter
		```
	
	- The previous two code examples were taken from the following TensorFlow tutorial website page: https://www.tensorflow.org/install

---

### Execution

How do you get the resource ready to use? Are there inputs to know? Please show a step-by-step guide (in a tutorial format) for readying the resource for your work. Include screenshots of successful execution and use of the software.

	- You can use TensorFlow in order to build a basic machine learning program. On the beginner tensorflow tutorial page (https://www.tensorflow.org/tutorials/quickstart/beginner) they discuss an example that I will be going into a deeper explanation of here.
	- In order to us=e the tensorflow library in your python program, you need to use the following import statement:
		```
		#import TensorFlow
		import tensorflow as tf
		```
		- While 'as tf' is not necessary for the library to work, many people use it as it makes the chances of errors due to spelling errors much less likely to occur.
	- You can now use the TensorFlow library in order to load in a dataset using the following code statements:
		```
		mnist = tf.keras.datasets.mnist

		(x_train, y_train), (x_test, y_test) = mnist.load_data()
		x_train, x_test = x_train / 255.0, x_test / 255.0
		```
		- These code statements do the following:
			- Using the TensorFlow library, you can assign a mnist database to a mnist variable.
			- Using the mnist variable, you can load in the data and create testing values.
	- Next, you will want to build the actual machine learning model for your program using the following code:
		```
		model = tf.keras.models.Sequential([
		tf.keras.layers.Flatten(input_shape=(28, 28)),
		tf.keras.layers.Dense(128, activation='relu'),
		tf.keras.layers.Dropout(0.2),
		tf.keras.layers.Dense(10)
		])
		```
		- In order to create a Sequential model, you need to shape the model and add the parameters you want.
	- You then can enter the following command to see what the log-odd scores are:
		```
		predictions = model(x_train[:1]).numpy()
		predictions
		```
		- When you run this, this is the output it gives you:
			```
			array([[ 0.2760778 , -0.39324787, -0.17098302,  1.2016621 , -0.03416392,
			0.5461229 , -0.7203061 , -0.41886678, -0.59480035, -0.7580608 ]],
			dtype=float32)
			```
	- You can use the tensorflow function softmax() in order to take the log-odds and turn them into probabilities:
		```
		tf.nn.softmax(predictions).numpy()
		```
		- When you run this, this is the output you get:
			```
			array([[0.11960829, 0.06124588, 0.0764901 , 0.30181262, 0.08770514,
			0.15668967, 0.04416083, 0.05969675, 0.05006609, 0.04252464]],
			dtype=float32)
			```
	- You can define a loss function to train your model using the function losses.SparseCategoricalCrossentropy(), which can tell you your loss for each of your log-odds.
		```
		loss_fn = tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True)
		```
		- The output, or the loss, is equal to zero if the model is of the correct class
	- For an untrained model, the output of the following command should be close to log(1/10), or 2.3. This is the chance of the 'correct' answer being chosen at random.
		```
		loss_fn(y_train[:1], predictions).numpy()
		```
		- When you run this command, you will get an answer around 2.3.
			```
			1.8534881
			```
	- This is how you can build a basic machine learning model! Once you finish these steps, you can train your model to make it accurate to the results you want.
	

---

### Helpful resources

Include some of the relevant resources (links, articles, etc.) that you used to write in your tutorial.

	- The TensorFlow website has extensive documentation to help you understand how to use their library. Some of the best links I found were:
		- https://www.tensorflow.org/tutorials/quickstart/beginner
		- https://www.tensorflow.org/overview/
		- https://www.tensorflow.org/guide/keras/sequential_model
		- https://www.tensorflow.org/tutorials/keras/classification