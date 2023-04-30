# Hurricane_harvey_UAV-Image-Segmentation

## Data
Please download the folders containing data files from this link:
<a>https://drive.google.com/drive/folders/1Soejx2LLTaNt42VkXi_RJi8LI5cIMzAw?usp=sharing</a>

Natural disasters can cause catastrophic damage, making it difficult for relief efforts to identify areas of need quickly. To address this problem, we built a semantic image segmentation model that identifies and localizes different assets in high-resolution photographs captured by small UAVs after a natural disaster. Specifically, we focus on post-Hurricane Harvey relief efforts in the Houston, Texas region.

## Project Overview
Our project involved building a multiclass segmentation model to identify and localize different assets in residential areas of Houston. We used masks for each image to label 27 different classes, including property roofs, swimming pools, vehicles, trees/shrubs, and water bodies. We applied various data preprocessing techniques and augmentations to enhance the image quality and enable accurate segmentation.

## Methodology
Our implementation process consisted of the following steps:
1. Data exploration
2. Data preprocessing
3. Image augmentations
4. Building and tuning the model with hyperparameters
5. Model evaluation
6. Predictions, resizing, and tar file creation

We developed various helper functions and classes for data loading, visualization, and preprocessing. To handle the varying dimensions of the images, we resized them to (352, 480) pixels each and used the preprocess_input function from the keras API. We also applied various augmentations using the Albumenations library, including horizontal flips, brightness/contrast/color manipulations, image blurring and sharpening, and Gaussian noise. We used the UNet model to achieve segmented high-resolution image outputs.

## Evaluation and Results
We ran several models with varying parameters and evaluated their performance using accuracy and loss curves. The SeResNet model gave the best result of 62.65% accuracy on the test set prediction. Below table provides all results:
![image](https://user-images.githubusercontent.com/29313860/235377400-06f06694-e3de-4d68-a9d1-30ad17a074f2.png)


## Conclusion
Our project demonstrates the potential of using semantic image segmentation to identify areas of need after a natural disaster quickly. With further development and refinement, this technique could become a valuable tool for post-disaster relief efforts.
