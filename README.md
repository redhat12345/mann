# mann
Robust Unsupervised Domain Adaptation via Moment Alignment

This repository contains code for reproducing the experiments reported in the paper
- W. Zellinger, B.A. Moser, T. Grubinger, E. Lughofer, T. Natschlaeger, and S. Saminger-Platz, "Robust unsupervised domain adaptation
for neural networks via moment alignment," submitted, 2017

that extends the preliminary conference version

- W.Zellinger, T. Grubinger, E. Lughofer, T. Ntschlaeger, and Susanne Saminger-Platz, "Central moment discrepancy (cmd) for domain-invariant representation learning," International Conference on Learning Representations (ICLR), 2017

# requirements
The implementation is based on the neural networks library keras (version 1.1) and tested with theano backend. For installing theano and keras please follow the installation instruction on the respective github pages. You will also need: numpy, pandas, seaborn, matplotlib, and scipy.

# datasets
In our paper, we report results for one artificial dataset and two benchmark datasets: AmazonReview and Office. In addition, the model weights of the AlexNet model pre-trained on Imagenet are used. The artificial dataset and the AmazonReviews dataset are provided. The Office data set can be downloaded from https://drive.google.com/file/d/0B4IapRTv9pJ1WGZVd1VDMmhwdlE/view. Copy the folders amazon, dslr and webcam to data/office_dataset/. Download the AlexNet weights file from http://files.heuritech.com/weights/alexnet_weights.h5 and copy it to  data/office_dataset/.

# experiments
Use the files, artificial_example.py, object_recognition.py, sentiment_analysis.py and parameter_sensitivity.py to run all the experiments and create all the images from the paper. Please note that the code runs the full grid searches and random restarts and can therefore run some days.

