### Classification Example 1

A simple caffe program for a toy classification problem. A animal or human toy image classification problem is used here. Dataset is prepared by taking the images from standard image datasets. A Lenet like CNN network is used. <br>

#### To run this example: <br>
Setting up:
1. Download [this](https://github.com/s9xie/hed) version of Caffe into a folder /path/to/caffe/ <br>
2. Install caffe and its dependencies by following the steps [here](http://caffe.berkeleyvision.org/installation.html).  <br>
3. Install pycaffe by running make pycaffe in /path/to/caffe/  <br>
4. Download the folder "Classification Example 1" and place it in /path/to/caffe <br>
5. Download the dataset from [here](https://drive.google.com/open?id=19az8rs-qKk8tGa6JzuXYbpUeRgZNz1_3) and place it inside the above folder <br>


For training:
1. Run the script example_train_test.py using the command: <br>
$ python example_train_test.py <br>

For testing:
1. Use caffe inbuilt tool: <br>
$ ../build/tools/caffe test -model ./example_train_test.prototxt -weights ./logdir/dnn_iter_200000.caffemodel -iterations 100 <br>

For deploying: <br>
1. Run the script example_deploy.py using the command: <br>
$ python example_train_test.py  (you may specify the image to use inside the python scipt) <br>
