# What is DeepForest-pytorch?
DeepForest-pytorch is a python package for training and predicting individual tree crowns from airborne RGB imagery. DeepForest-pytorch comes with a prebuilt model trained on data from the National Ecological Observatory Network. Users can extend this model by annotating and training custom models.

![](../www/image.png)

# What is the difference between DeepForest-pytorch and the original DeepForest?

The original project https://deepforest.readthedocs.io/ was written in tensorflow based on keras-retinanet. When tensorflow updated to 2.0 there were breaking changes and the authors of keras-retinanet decided to not attempt to recover the project. 
The rapid development of open machine learning community resources means that tensorflow 1.1.14, which is required for deepforest, will rapidly become out of date. 
As of 3/12/2021 there are no current no breaking changes, but the potential for them will increase over time. Unless there is a compelling interest, this project should be used and the release model will be updated here and not in the original tensorflow version.


## How does deepforest-pytorch work?

DeepForest uses deep learning object detection networks to predict bounding boxes corresponding to individual trees in RGB imagery. 
DeepForest is built on the retinanet model from the [torchvision package](http://pytorch.org/vision/stable/index.html) and designed to make training models for tree detection simpler.

## Demo
For a quick example of model performance on sample images, see our demo shiny app. Please note that the model continues to improve and the app model may not reflect results from the current release.

[http://tree.westus.cloudapp.azure.com/trees/](http://tree.westus.cloudapp.azure.com/trees/)

## License
Free software: [MIT license](https://github.com/weecology/DeepForest/blob/master/LICENSE)

## Why DeepForest?
Remote sensing can transform the speed, scale, and cost of biodiversity and forestry surveys. Data acquisition currently outpaces the ability to identify individual organisms in high resolution imagery. Individual crown delineation has been a long-standing challenge in remote sensing and available algorithms produce mixed results. DeepForest is the first open source implementation of a deep learning model for crown detection. Deep learning has made enormous strides in a range of computer vision tasks but requires significant amounts of training data. By including a trained model, we hope to simplify the process of retraining deep learning models for a range of forests, sensors, and spatial resolutions.

## Feedback
All [issues](https://github.com/weecology/DeepForest-pytorch/issues/) can be submitted to the github repo. We look forward to hearing about the performance of the prebuilt and custom models. 

## Citation

[Weinstein, B.G.; Marconi, S.; Bohlman, S.; Zare, A.; White, E. Individual Tree-Crown Detection in RGB Imagery Using Semi-Supervised Deep Learning Neural Networks.
Remote Sens. 2019, 11, 1309](https://www.mdpi.com/2072-4292/11/11/1309)

[Geographic Generalization in Airborne RGB Deep Learning Tree Detection Ben Weinstein, Sergio Marconi, Stephanie Bohlman, Alina Zare, Ethan P White
bioRxiv 790071; doi: https://doi.org/10.1101/790071](https://www.biorxiv.org/content/10.1101/790071v1.abstract)
