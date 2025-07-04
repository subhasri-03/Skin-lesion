Skin Lesion Classification using ResNet50 + XGBoost

This project focuses on classifying skin lesions into 7 types using deep learning with transfer learning (ResNet50) and boosting techniques. It uses the HAM10000 dataset, part of the ISIC archive of dermoscopic images.

🔍 Features

✅ Transfer Learning with ResNet50 (ImageNet weights)

✅ Data Augmentation and Preprocessing

✅ Class Imbalance handled using class weights

✅ Evaluation using Classification Report & Confusion Matrix

✅ Final test accuracy above 90%

✅ Model saved and reused with .h5 format

✅ Ready for Deployment with Streamlit or Flask

🗂️ Folder Structure

SkinLesion-Classification/
├── model/
│   └── saved_skinlesionmodel.h5
├── dataset/
│   ├── HAM10000_metadata.csv
│   └── HAM10000_images/
├── src/
│   ├── train.py
│   └── predict.py
├── deploy/
│   └── app.py (for Streamlit or Flask deployment)
├── requirements.txt
├── README.md
└── .gitignore

📦 Installation

pip install -r requirements.txt

🚀 How to Use

🔧 Train the model

cd src
python train.py

🔍 Predict on new images

python predict.py --image path_to_image.jpg

🧠 Model Performance

Accuracy: ~94% on test dataset

Evaluation: Precision, Recall, F1-score per class

Confusion matrix and loss/accuracy curves included

📊 Dataset

HAM10000 from ISIC Archive: Kaggle Dataset

7 Classes: nv, mel, bkl, bcc, akiec, vasc, df

🖼 Sample Output

Model Accuracy Plot

Model Loss Plot

Confusion Matrix Heatmap

Classification Report

📤 Deployment (Optional)

You can use Streamlit or Flask to build a user-friendly web interface.

cd deploy
streamlit run app.py

✍️ Author

Subhasri P

📃 License

This project is open source and available under the MIT License.
