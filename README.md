# Tensorflow
## Installation of tensorflow on MacOS
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

Exit docker
#control-D
