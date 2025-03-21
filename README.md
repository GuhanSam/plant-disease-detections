# Plant Disease Detection using CNN

## Problem Description
Plant diseases can significantly affect crop yield and quality, leading to economic losses. Farmers often struggle to identify diseases accurately, resulting in improper treatment. This project aims to develop an AI-based solution to detect plant diseases from images and provide relevant information about the disease along with suitable fertilizers for treatment.

## Solution
This project uses a Convolutional Neural Network (CNN) trained on the **PlantVillage dataset** to classify plant diseases. The system allows users to upload an image of a plant leaf, and the model predicts the disease, providing a description, preventive measures, and recommended fertilizers.

## Libraries Used
- **Flask**: For building the web application.
- **Torch & Torchvision**: For deep learning and model inference.
- **Pandas**: For handling dataset information.
- **PIL (Pillow)**: For image processing.
- **NumPy**: For numerical computations.

## Algorithm & Model Details
### CNN Architecture
The model is built using a Convolutional Neural Network (CNN) and trained on the **PlantVillage dataset**.

1. **Input Layer**: Accepts an image resized to `224x224` pixels.
2. **Convolutional Layers**: Extracts features using multiple convolutional layers with ReLU activation.
3. **Pooling Layers**: Reduces spatial dimensions to retain key features.
4. **Fully Connected Layers**: Classifies the image into one of the 39 plant disease categories.
5. **Softmax Activation**: Outputs probability scores for each class.

### Model Performance
- **Training Accuracy**: 96.7%
- **Test Accuracy**: 98.9%
- **Validation Accuracy**: 98.7%

## How the Project Works
1. The user uploads an image of a plant leaf via the web application.
2. The model processes the image and predicts the disease.
3. The system retrieves disease-related information, including:
   - Disease name
   - Description
   - Preventive measures
   - Suggested fertilizers with images and purchase links
4. The results are displayed on the webpage.

## Project Workflow
1. **User uploads an image** of a plant leaf.
2. The **Flask backend processes the image** and sends it to the **CNN model**.
3. The **model predicts the disease** and retrieves relevant information from `disease_info.csv` and `supplement_info.csv`.
4. The results, including the **disease name, description, prevention steps, and recommended fertilizers**, are displayed on the webpage.
5. Users can **purchase the recommended fertilizers** using the provided links.

## Future Enhancements
- Improve model accuracy with additional training data.
- Add real-time image capture for mobile users.
- Deploy the model as a cloud-based API for integration with mobile apps.

## ( Dataset link):
<a href="https://medium.com/analytics-vidhya/plant-disease-detection-using-convolutional-neural-networks-and-pytorch-87c00c54c88f" target="_blank">Plant Disease Detection using Convolutional Neural Network with PyTorch Implementation</a>
