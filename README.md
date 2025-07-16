# My-Project Cassava Leaves Disease Classifcation
🌿 Cassava Leaf Disease Classification
This repository contains implementations of multiple deep learning models for the Cassava Leaf Disease Classification Kaggle competition.

📌 Problem Statement
The objective is to classify images of cassava leaves into five classes:

Cassava Bacterial Blight (CBB)

Cassava Brown Streak Disease (CBSD)

Cassava Green Mottle (CGM)

Cassava Mosaic Disease (CMD)

Healthy

Accurate classification helps farmers detect diseases early and improve yield outcomes.

🗃️ Dataset
Source: Cassava Leaf Disease Classification | Kaggle

Download Command:

bash
Copy
Edit
kaggle competitions download -c cassava-leaf-disease-classification
The dataset includes:

train_images/ : Folder with training images.

train.csv : Labels for training data.

test_images/ : Folder with test images.

sample_submission.csv : Sample format for submission.

🛠️ Models Implemented
1. EfficientNet
Used transfer learning with EfficientNet architecture for improved performance with fewer parameters.

Fine-tuned on cassava dataset to leverage pre-trained ImageNet features.

2. LeNet
Implemented classical LeNet-5 architecture for baseline comparison.

Observed limited performance due to shallow architecture, included for theoretical learning.

3. ResNet
Implemented ResNet with skip connections to mitigate vanishing gradient problems.

Improved learning of deeper representations.

4. VGG
Used VGGNet architecture for its simplicity and powerful feature extraction capability.

🧪 Results
Model	Key Observations
LeNet	Low accuracy due to simple architecture, not suitable for this complex dataset.
VGG	Better than LeNet but heavy on parameters.
ResNet	Good performance due to residual connections enabling deeper learning.
EfficientNet	Best results leveraging scaling and transfer learning.

🔧 Models Implemented
Model Name	    Validation Accuracy (%)	    Final Loss	  Epochs
EfficientNetB3	      84.69                  	0.4435	      5
LeNet	                61.47                  	1.1229	     10
ResNet50	            61.96                  	1.1225	     10
VGG16                	69.53                  	1.0610       10

(Add your model-wise accuracy or validation metrics here after running your notebooks.)

⚙️ Usage
Clone this repository:

bash
Copy
Edit
git clone https://github.com/<your-username>/cassava-leaf-disease-classification.git
cd cassava-leaf-disease-classification
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Download dataset using:

bash
Copy
Edit
kaggle competitions download -c cassava-leaf-disease-classification
unzip cassava-leaf-disease-classification.zip
Run any of the notebooks:

EfficientNet.ipynb

LeNet.ipynb

ResNet.ipynb

VGGCassava.ipynb

🚀 Future Work
Hyperparameter tuning for each architecture.

Implementing ensemble models for improved accuracy.

Deployment as a streamlit web app for farmer use.

🤝 Contributing
Contributions are welcome! Please open an issue to discuss improvements or raise a PR.

📄 License
This project is open-source under the MIT License.

✨ Acknowledgements
Kaggle for dataset and competition platform.

TensorFlow/Keras/PyTorch frameworks used in this project.
