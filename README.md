# Semantic_Segmentation
Semantic Segmentation is an image analysis procedure in which we classify each pixel in the image into a class.
identifying and separating each of the objects in an image and labeling them accordingly.

Pipeline:
1. Data building/preprocessing link: https://towardsdatascience.com/creating-and-training-a-u-net-model-with-pytorch-for-2d-3d-semantic-segmentation-dataset-fb1f7f80fe55 1.1 data transformations: normalization, centercrop, resize, toTensor  1.2 data augmentation (we have 113 test images and 262 train images  bonus: how to make edges more evident reduce the solution 
2. Define a model   Model choices: 2.1 U-net  https://www.pyimagesearch.com/2021/11/08/u-net-training-image-segmentation-models-in-pytorch/ 2.2 Masked RNN  Bonus: transfer learning for faster convergence packaged modules: https://github.com/qubvel/segmentation_models.pytorch tutorial: https://medium.com/@seymatas/pytorch-image-segmentation-tutorial-for-beginners-i-88d07a6a63e4?source=search_post---------0------------------------------- 
3. Training 
4. Prediction

Additional work: https://towardsdatascience.com/creating-and-training-a-u-net-model-with-pytorch-for-2d-3d-semantic-segmentation-training-3-4-8242d31de234 1. Hyperparameter Tuning   1.1 find best learning rate
try a different optimizer like Adam instead of SGD, 
use different activation functions, 
increase the number of kernels, 
use different normalization layers, 
different upsampling methods ….. 2. Improve on data loader to speed up epochs   2.1 load into caches when needed 



