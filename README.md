There are two methods for pulling images from a directory on your machine the ImageDataGenatros that is used with image from directory or the tf.keras.preprocessing image from directory which this model uses. Therefore i have an augmentation method 
which handels data augemdntation. Its worth noting that ImageDataGenators does augmentation on the fly while training but i´ve experimened with a different method here. The big difference this model uses a bespoke Resnet model with an input layer, 
a entry block of layers that enable layer skipping to avoid hitting the threshold e.g. all CNNs have a threshold of layers where after a given layer the performance degrades. This skipping of layers avoids such a problem.
