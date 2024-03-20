# Veterinary Bacteria Classification Using Deep Learning 🦠🔬

## Introduction
In the field of medical research, accurate identification and classification of bacteria from images play a crucial role in diagnosis and treatment. This project focuses on developing a robust multiclass classification system using image datasets. Through a series of preprocessing steps, model training, and evaluation, we aim to contribute to the advancement of medical diagnostic tools.

To address the automation of bacteria classification by convolutional neural networks in our work, we have considered the cultured 24 bacteria species (classes) from a total of 56,865 images.

## Motivation
The need for precise classification of bacteria stems from its direct impact on patient care and public health. By accurately identifying bacterial strains, healthcare professionals can tailor treatment plans, anticipate antibiotic resistance patterns, and mitigate the risk of spreading infectious diseases. Moreover, an automated classification system can streamline the diagnostic process, leading to faster interventions and improved patient outcomes.

## Dataset 📊
Our dataset consists of annotated images depicting various bacterial strains commonly encountered in medical settings. These images were meticulously curated and annotated to ensure accuracy and relevance to the target classification task. The dataset covers a wide range of bacterial species, enabling comprehensive model training and evaluation.

## Methodology 🛠️
### Data Preprocessing
1. **Image Cropping**: Images were cropped according to annotations to focus on relevant bacterial regions.
2. **Image Padding**: To standardize image dimensions, padding was applied to ensure uniformity across the dataset.
3. **Image Augmentation**: Augmentation techniques such as rotation, flipping, and scaling were employed to increase dataset variability and improve model generalization.

### Model Architecture 🧠
We employed a set of pre-trained deep-learning models on a dataset of bacterial colony images, fine-tuned on our dataset. The models included:
- XceptionNet
- InceptionResNetV2
- ResNet-50
- InceptionV3
- MobileNetV2
- EfficientNet-B0 to B7

### Model Training 🚀
Each model was fine-tuned on the bacterial colony dataset and evaluated for its classification accuracy. For initial training purposes, we used the Nadam optimizer with a learning rate of 0.001 combined with the reduction on plateau having factor 0.2 and patience 3. A batch size of 32 was used, and categorical cross-entropy loss.

All training and validation processes were carried out using P100 GPUs. The data in Tables 3 and 4 are for fine-tuning the specific models on our dataset for 20 epochs.

## Results 📈

The EfficientNetB4 model achieved a commendable accuracy of over 90% on the test dataset, demonstrating its effectiveness in classifying bacterial strains. The model exhibited robustness across various evaluation metrics, indicating its potential for real-world deployment in medical settings. Furthermore, comparative analyses with other pretrained models underscored the superiority of EfficientNetB4 in terms of both accuracy and computational efficiency.

## Conclusion 🎉
In conclusion, this project highlights the significance of automated multiclass classification systems in medical research, particularly in the domain of bacterial identification. By leveraging annotated image datasets and state-of-the-art deep learning models, we have demonstrated the feasibility of accurate and efficient bacteria classification. Our findings pave the way for further advancements in medical diagnostics and underscore the transformative potential of artificial intelligence in healthcare.


### Authors
- Sneh Shah
- Neel Shah
- Pankil Soni
- Dhaval Patel
- Dr. Nirav Bhatt
