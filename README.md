# OCR-GPU-to-CPU-Evaluation

This code implements a convolutional neural network (CNN) using PyTorch to classify handwritten characters from the EMNIST dataset. It begins by unzipping the dataset and defining a SimpleCNN model with two convolutional layers, dropout for regularization, and fully connected layers. The model is trained on a GPU for two epochs, and its performance is evaluated on both GPU and CPU using Intel's OpenVINO toolkit for inference optimization. The code also measures training time, accuracy, and frames per second (FPS) for both GPU and CPU inference, providing insights into the model's efficiency and effectiveness.

Performance metrics-

GPU Training Performance:

Training Time: 52.58 seconds

Inference Accuracy: 85.37%

Inference Time: 3.78 seconds

Frames Per Second (FPS): 4967.58


CPU (OpenVINO) Inference Performance:

Inference Time: 5.88 seconds

Inference Accuracy: 85.37%

FPS: 3195.59

**Since I ran this code on Kaggle, it's important to note that the free version utilizes an Intel Xeon processor from 2012, operating at a frequency of only 2.00 GHz and based on an older architecture. Consequently, the CPU performance does not match that of the GPU. However, if this model is used for inference on more recent mainstream Intel CPUs, such as the Core i series (i3, i5, i7, i9), it may yield improved inference and frames per second (FPS) performance.
