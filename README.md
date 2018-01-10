# Docker and Tensorflow
## Installation of Docker on Mac OS
### Install docker
```
Download the Docker installer here.
Mount ‘Docker.dmg’
Copy Docker.app to your Application directory
Double click Docker.app and wait for Docker to finish starting up
Open terminal and run the docker hello-world image
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

### Exit docker
```
Control-D
```
