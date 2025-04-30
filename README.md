# RetinaxCrossModal
![dr-convnet-small](https://github.com/user-attachments/assets/489dea8a-6556-4e35-9c01-7eb8226e6bfd)

# Abstract 
Diabetic retinopathy (DR) is a diabetes-related eye disease that can lead to vision loss. Early detection is vital. This study compares Vision Transformers (ViT), ResNet, and MobileNet for DR classification using a balanced dataset combining APTOS-2019, Diabetic Retinopathy Preprocessed (256x256), and the Diabetic Retinopathy Arranged dataset the latter used to train GANs for synthetic image generation. Results show ResNet achieving a validation F1-score of 0.7617, outperforming MobileNet’s 0.7186. This work highlights the strengths and trade-offs of each model, aiming to enhance automated DR screening and support early diagnosis.
<br>

# Dataset
- https://www.kaggle.com/datasets/mariaherrerot/aptos2019<br>
- https://www.kaggle.com/datasets/amanneo/diabetic-retinopathy-resized-arranged
- https://www.kaggle.com/datasets/sachinkumar413/diabetic-retinopathy-dataset

# Methodology <br>
- <B>Data Augmentation</B>: Applied random rotations, scaling, contrast shifts, and flips to improve model robustness.<br>
- <B>Model Architectures</B>: Compared ViT, ResNet50, and MobileNetV2, all pre-trained on large image datasets.<br>
- <B>Class Imbalance Handling</B>: Used class-balanced filtering and WeightedRandomSampler with computed class weights.
<br>
<p align="center">
  <img src="https://github.com/user-attachments/assets/d218490f-be70-4223-8b2d-cb1151152480" width="48%" />
  <img src="https://github.com/user-attachments/assets/72399444-b9ae-46fe-915a-ae4b40e461d3" width="48%" />
</p>

### Performance Comparison of Tested Models on the Data

|     MODEL     |   Loss (Train)   |   F1 Score (Train)   |   Loss (Validation)   |   F1 Score (Validation)   |
|:-------------:|:----------------:|:---------------------:|:----------------------:|:--------------------------:|
|     VIT       |     0.3016       |        0.9021         |        0.5401          |           0.8251           |
|   RESNET      |     0.2948       |        0.7803         |        0.8758          |           0.7617           |
|  MOBILENET    |     0.5122       |        0.6517         |        0.8758          |           0.7186           |





  
