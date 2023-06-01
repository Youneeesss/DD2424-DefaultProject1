# DD2424-DefaultProject1

The goal of this project was to explore the possibilities of transfer learning by fine-tuning
a pre-trained convolution model and making it perform on a different dataset. The idea is
that, during training, we only update the parameters of a few specific layers, whereas the
rest of the pre-trained weights remain frozen. According to many papers, this approach
yields better results than training a model from scratch and also reduces the training cost.

In the first part of the project, we decided to apply this method to the Oxford PET
dataset, with both a binary classification (distinguishing between images of cats and dogs)
and a multi-classification problem (identifying the breed). To do this, we used Resnet50 as
our base and applied several fine-tuning steps to improve performance.

The second part was dedicated to semi-supervised learning. We wanted to see what
techniques existed to train a model with missing labels, and which one was most efficient. We
only implemented 2 different methods, Consistency Regularization, and Pseudo-Labeling,
and ran them on the PET dataset which we removed more and more labels.
