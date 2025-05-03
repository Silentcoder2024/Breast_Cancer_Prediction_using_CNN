# Breast_Cancer_Prediction_using_CNN
This project presents a deep learning-based breast cancer classification and staging system developed using a customized ResNet-18 model and K-Means clustering. The system is designed to classify microscopic breast cell images as benign or malignant, and further estimate the cancer stage (1 to 4) for malignant cases to support early diagnosis and treatment planning.

We trained the ResNet-18 model on a dataset of over 6000 labeled images, where filenames ending in _class0 indicated benign samples and _class1 indicated malignant ones. The model leverages convolutional layers and residual connections to extract high-level features from the images and achieve robust classification performance.

Since the dataset lacked explicit cancer stage labels, we applied K-Means clustering on feature representations of the malignant images (extracted using the trained ResNet-18) to group them into four clusters. These clusters were interpreted as cancer stages 1 through 4, based on visual and structural complexity in the images.

🔍 Key Features:
✅ Accurate classification of breast cell images as benign or malignant

📊 Unsupervised prediction of cancer stage using K-Means clustering

📁 Simple image naming-based labeling (_class0, _class1)

🖼️ User interface for uploading images and getting real-time predictions

🤖 Built using PyTorch, OpenCV, scikit-learn, and ResNet-18

This system demonstrates how deep learning and unsupervised learning can be combined to build intelligent medical imaging tools that assist in early cancer detection and stage estimation.
