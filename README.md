# Sat-Images-water-Body-Segmentation-model-from-scratch

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

* I tried in the first file Mean IOU and binary_crossentopy as the loss.

* I tried in the second notebook **model_from_scratch_2** a **weighted dice loss** that I defined to use the class weights for reference and an defined IOU but gave me the loss with negative values, I also didn't apply **Augmentation**.

* In the last notebook, I applied **Augmentation**, modified the **dice loss** so that it won't be with the weights, and fitted another model with loss of **binary_crossentropy**

### For all notebooks

* Matched the correct masks to images, since there are more masks than images in the dataset folder.

* I applied Min Max Scaler for Normalization instead of dividing by 255 because for some bands, the pixel intensity is above 255.

* Visualized each band of the images

* Implemented a Unet Model from scratch with about 41 million paramters to try to work well with the data using `Tensorflow` and `Keras`

* Visualized the Model's **accuracies**, **losses** and **IOU** curves.

* Evaluated the model by **IOU**, **rcall**, **precision**, **f1 score** metrics

* Visualized the `Satellite Image`, `Ground Truth Mask` and the `Predicted Mask`.  
