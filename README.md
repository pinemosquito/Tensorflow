# Docker and Tensorflow
## Installation of Docker on Mac OS
### Install docker
```
Download the Docker installer
Mount ‘Docker.dmg’
Copy Docker.app to your Application directory
Double click Docker.app and wait for Docker to finish starting up
Open terminal and run the docker hello-world image
Verify Version 17.09.1-ce-mac42
```


## Installation of tensorflow on Mac OS
### Install tensorflow

```
From terminal,
docker run -it gcr.io/tensorflow/tensorflow:latest-devel
You should see root@xxxxxxxxxxxx# which means docker is running
```

### Test installations

```
python
>>>import tensorflow as tf
>>>hello = tf.constant('Hello, TensorFlow!')
>>>sess = tf.Session()
>>>print(sess.run(hello))
If you see Hello, TensorFlow! Then it works
quit() to leave Python shell
```

### Eager Installation
You will need version 1.5.0 to install Eager.  My version of Tensorflow was 0.1.2
```
$docker run -it gcr.io/tensorflow/tensorflow:latest-devel
root@37eec9a002ca:~# 
This means installation is successful and docker is running
#python
>>>import tensorflow as tf
>>>tf.__version__
1.5.0
>>quit() 
#control-D
```

### Pulling docker image 
Open terminal
```
docker pull tensorflow/tensorflow
```
test image
```
docker run -it -p 8888:8888 tensorflow/tensorflow
```

### Cloning repo
Clone github repo  https://github.com/aamini/introtodeeplearning_labs

Unzip folder to anywhere you like.  I will assume it is located at ~/desktop/introtodeeplearning_labs-master

Open terminal 
```
docker pull tensorflow/tensorflow
```
test image
```
docker run -it -p 8888:8888 -v ~/desktop/introtodeeplearning_labs-master:/notebooks tensorflow/tensorflow
```
in browser, navigate to URL provided by docker


### Exit docker
```
Control-D
```
