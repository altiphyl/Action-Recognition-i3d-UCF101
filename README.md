# Action-Redognition-i3d-UCF101

This is an implementation of the following paper:

Carreira, Joao, and Andrew Zisserman. "Quo vadis, action recognition? a new model and the kinetics dataset." proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2017.

The reason I decided to implement this specific paper is because of their use of the i3d model. This model is pre-trained on the new Kinetics Human Action Video dataset. Kinetics has two orders of magnitude more data, with 400 human action classes and over 400 clips per class, and is collected from realistic, challenging YouTube videos.

For image data a CNN is the best neural net architecture to work with, in this paper they take it one step ahead by introducing a new Two-Stream Inflated 3D ConvNet (I3D) that is based on 2D ConvNet inflation: filters and pooling kernels of very deep image classification ConvNets are expanded into 3D, making it possible to learn seamless spatio-temporal feature extractors from video while leveraging successful ImageNet architecture designs and even their parameters.

Testing :  I tested the model on 3 different videos, 1 from the UCF101 dataset and 2 randomly picked from youtube.

video 1 : It was able to correctly identify the action from a clear video.

video 2 : It was able to correctly identify the action from a video, despite a mirror behind the subject causing 2 overlapping moving targets.

video 3 : It was able to correctly identify the action from a video, despite the video intro, multiple cut scenes and scene changes.
