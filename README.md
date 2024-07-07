# a-two-stage-attention-based-feature-enhancement-network-for-strip-steel-surface-defect-detection
This module effectively captures contextual information and enhances the representation of the fused features.
the first-stage feature-enhancement procedure (FSFE) utilizes an AC fusion module with convolution to combine all four-level features and then strengthens the features of different levels via an RSC attention module. The second-stage feature-enhancement procedure (SSFE) combines three-level features using an AS fusion module with self-attention and then strengthens the features using an RSC attention module. Experiments on the NEU-DET and GC10-DET datasets demonstrated that the proposed method significantly improved detection accuracy
The proposed method was implemented using the
Ubuntu operating system with an Intel(R) Xeon(R) CPU
E5-2650 v4 @ 2.20 GHz processor and four TITAN Xp
GPUs. The PyTorch deep learning framework was uti-
lized for the implementation. During the training of the
NEU-DET dataset, the image sizes were adjusted to 224
× 224 pixels, and for the GC10-DET dataset, the image
sizes were adjusted to 512 × 512 pixels. In both cases,
the datasets were randomly divided in a 7:1:2 ratio to gen-
erate the training, validation, and test sets. The NextVit
backbone was initialized with a pretrained weight trained
on the ImageNet dataset. The stochastic gradient descent
with an initial learning rate of 0.01 and a weight decay of
0.0005 was used as the optimizer. During the training pro-
cess, various data augmentation techniques were applied
to enhance the performance of the model. These tech-
niques include horizontal flipping, affine transformation,
mosaicism, hue changes, brightness changes, and satura-
tion changes. The model was trained for 300 epochs using
the augmented datasets.
