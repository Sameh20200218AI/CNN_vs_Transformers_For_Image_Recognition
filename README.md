# Image Recognition Project: CNN vs Transformers

## Project Overview
This project focuses on image recognition using both Convolutional Neural Networks (CNNs) and Vision Transformers (ViTs). The dataset used in this project contains images classified into four weather conditions: **Cloudy, Rain, Shine, and Sunrise**.

## Libraries and Tools Used
- `cv2` for image processing
- `pandas` and `numpy` for data handling
- `PIL` (Pillow) for image manipulation
- `transformers` for implementing Vision Transformer models
- `tensorflow/keras` for deep learning model implementation
- `sklearn` for data preprocessing and evaluation
- `seaborn` and `matplotlib` for data visualization

## Data Preprocessing
- The images were resized to a fixed size of **224x224** pixels.
- Normalization was applied to the images for better model performance.
- The dataset was split into **80% training and 20% testing**.
- The dataset distribution was visualized using **bar charts** and **pie charts**.
- The training dataset initially had **898 images**, and the testing dataset had **225 images**.
- **Data Augmentation** was applied, increasing the training dataset to **1,796 images**.

## Model Training and Performance

### CNN Models (Pretrained Architectures)
| Model            | Test Accuracy |
|-----------------|--------------|
| ResNet50        | 0.5288       |
| MobileNetV2     | 0.9422       |
| VGG16           | 0.9155       |
| VGG19           | 0.9066       |
| InceptionV3     | 0.9111       |
| EfficientNetB0  | 0.2977       |
| ConvNeXtSmall   | 0.4444       |

### Vision Transformer (ViT) Models
| Model                    | Test Accuracy |
|--------------------------|--------------|
| Fine-tuned Pretrained ViT | 0.9244       |
| ViT from Scratch         | 0.9378       |

## Results & Conclusion
- **MobileNetV2 achieved the highest accuracy (94.22%)** among CNN models.
- **ViT from Scratch outperformed CNN models with 93.78% accuracy**, proving that Vision Transformers can be highly effective in image recognition tasks.
- **Pretrained ViT achieved 92.44% accuracy**, demonstrating that transfer learning can be beneficial in transformer-based image recognition.
- **ResNet50 and EfficientNetB0 performed poorly**, indicating that some CNN architectures might not be well-suited for this dataset.

![CNN vs Transformers](https://github.com/Sameh20200218AI/CNN_vs_Transformers_For_Image_Recognition/blob/main/CNN%20vs%20Transformers.png)

This study highlights the strengths of **CNNs and Vision Transformers**, showcasing how Transformers are emerging as powerful alternatives for image recognition tasks.

