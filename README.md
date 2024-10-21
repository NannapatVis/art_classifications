# **ClassPic (Art Image Classification using CNN)**

**Dataset:**  
Art Images: Drawing/Painting/Sculptures/Engravings [Click here](https://www.kaggle.com/datasets/thedownhill/art-images-drawings-painting-sculpture-engraving) 

##### Detail:  
Dataset with about 9,000 images containing 5 types of arts:
1. Drawings and watercolours
2. Works of painting
3. Sculpture
4. Graphic Art
5. Iconography (old Russian art)

## Model Comparison

In this project, several models were used to evaluate and compare their performance on the test images. The models utilized include:

- **VGG16**
- **VGG19**
- **InceptionV3**
- **MobileNetV2**

Each model was tested to assess its effectiveness in classifying artistic representations, providing insights into their respective strengths and weaknesses in handling non-standard image data.

**All processes and methods can be found in the model [VGG16](https://github.com/NannapatVis/art_classifications/blob/main/Train_IMGVGG16.ipynb), [VGG19](https://github.com/NannapatVis/art_classifications/blob/main/Train_IMGVGG19.ipynb), [InceptionV3](https://github.com/NannapatVis/art_classifications/blob/main/InceptionV3-3.ipynb), and [MobileNetV2](https://github.com/NannapatVis/art_classifications/blob/main/Train_IMGMobileNetV2.ipynb).**

## Test Images

![Test Image](./testPic.jpg)

## Test Results Summary

| Model          | Time (minutes) | Training Phase | Test Set        | Training Accuracy | Training Loss | Validation Time | Validation Accuracy | Validation Loss |
|----------------|----------------|----------------|------------------|-------------------|---------------|------------------|--------------------|------------------|
| **VGG16**      | 30:39          | 3:23           | 1:05             | 88.90%            | 0.303         | 0:45             | 96.60%             | 0.122            |
| **VGG19**      | 39:24          | 4:24           | 0:15             | 86.10%            | 0.424         | 0:46             | 94.72%             | 0.178            |
| **InceptionV3**| 28:41          | 4:02           | 0:57             | 64.95%            | 1.937         | 0:18             | 14.02%             | 4.183            |
| **MobileNetV2**| 4:17           | 0:39           | 0:11             | 91.82%            | 0.477         | 1:50             | 98.87%             | 0.039            |

## Test Results Summary (Single Image Prediction)

| Model          | Drawing | Engravings | Sculptures | Painting | Iconography | Predicted Class |
|----------------|---------|------------|------------|----------|-------------|------------------|
| **VGG16**      | 31.49%  | 0.75%      | 7.77%      | 54.29%   | 5.70%       | painting          |
| **VGG19**      | 0.05%   | 0.01%      | 0.86%      | 97.03%   | 2.04%       | painting          |
| **InceptionV3**| 14.44%  | 18.66%     | 23.84%     | 23.90%   | 19.16%      | painting          |
| **MobileNetV2**| 0.06%   | 0.00%      | 0.00%      | 99.36%   | 0.58%       | painting          |


## Acknowledgements

This project utilizes code from the following repository:

[Animal Image Classifications by Imamun93](https://github.com/imamun93/animal-image-classifications/tree/master)

The code used in this project is based on the implementation provided in the repository. The dataset used in this project, however, is different from the one in the original repository.
