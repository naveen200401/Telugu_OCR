Here is the Google Drive link for DATASET: https://drive.google.com/drive/folders/1RU_0nXY_4JOhsm6j-hYWKq7ms__3znLc?usp=sharing
# Telugu OCR (Optical Character Recognition)

A deep learning-based Optical Character Recognition system specifically designed for Telugu script, enabling accurate text extraction from images containing Telugu text.

## 🎯 Project Overview

This project implements a custom OCR solution for Telugu language text recognition, addressing the challenges of recognizing complex Indic scripts. The system uses computer vision and deep learning techniques to detect and recognize Telugu characters from images.

## ✨ Features

- **Telugu Script Recognition**: Specialized model trained for Telugu character recognition
- **Image Preprocessing**: Advanced image processing pipeline for better accuracy
- **Character Segmentation**: Intelligent segmentation of Telugu characters and words
- **Real-time Processing**: Fast inference for real-time applications
- **Multiple Input Formats**: Supports various image formats (JPG, PNG, etc.)
- **High Accuracy**: Optimized for Telugu script with competitive accuracy rates

## 🛠️ Technologies Used

- **Python**: Core programming language
- **TensorFlow/PyTorch**: Deep learning framework
- **OpenCV**: Image processing and preprocessing
- **NumPy**: Numerical computations
- **Matplotlib**: Visualization of results

## 📋 Prerequisites

- Python 3.7 or higher
- pip package manager
- GPU (optional, for faster training/inference)

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/naveen200401/Telugu_OCR.git
cd Telugu_OCR
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

## 💻 Usage

### Basic Usage

```python
from telugu_ocr import TeluguOCR

# Initialize the OCR model
ocr = TeluguOCR()

# Load and process an image
image_path = "path/to/your/telugu_image.jpg"
result = ocr.recognize(image_path)

# Print recognized text
print("Recognized Text:", result)
```

### Command Line Usage

```bash
python ocr_main.py --image path/to/image.jpg --output output.txt
```

## 📁 Project Structure

```
Telugu_OCR/
├── data/                   # Training and test data
├── models/                 # Trained model files
├── preprocessing/          # Image preprocessing modules
├── training/              # Model training scripts
├── utils/                 # Utility functions
├── ocr_main.py           # Main OCR script
├── requirements.txt       # Project dependencies
└── README.md             # Project documentation
```

## 🔄 Workflow

1. **Image Input**: Load Telugu text image
2. **Preprocessing**: 
   - Grayscale conversion
   - Noise reduction
   - Binarization
   - Skew correction
3. **Text Detection**: Locate text regions in the image
4. **Character Segmentation**: Segment individual characters
5. **Recognition**: CNN-based character recognition
6. **Post-processing**: Combine characters into words and sentences
7. **Output**: Return recognized Telugu text

## 🎓 Model Architecture

The OCR system uses a Convolutional Neural Network (CNN) architecture optimized for Telugu character recognition:

- **Input Layer**: Preprocessed character images
- **Convolutional Layers**: Feature extraction from Telugu characters
- **Pooling Layers**: Dimensionality reduction
- **Fully Connected Layers**: Classification
- **Output Layer**: Telugu character predictions

## 📊 Performance

- **Character Accuracy**: ~XX% (update with your metrics)
- **Word Accuracy**: ~XX% (update with your metrics)
- **Processing Speed**: X images/second
- **Supported Characters**: All Telugu Unicode characters

## 🔧 Training (Optional)

To train the model on your own dataset:

```bash
python train.py --data data/training --epochs 50 --batch_size 32
```

## 📝 Dataset

- Training dataset consists of Telugu text images
- Characters cover the complete Telugu Unicode range
- Images include various fonts, sizes, and quality levels

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🐛 Known Issues

- Performance may vary with handwritten Telugu text
- Requires good image quality for optimal results
- Complex ligatures may need additional training

## 🔮 Future Enhancements

- [ ] Support for handwritten Telugu text
- [ ] Mobile application integration
- [ ] Real-time video text recognition
- [ ] Multi-language support (Telugu + English)
- [ ] Web-based interface
- [ ] API deployment

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**Thupakula Naveen Chandu**

- GitHub: [@naveen200401](https://github.com/naveen200401)
- LinkedIn: [naveen-chandu-thupakula](https://www.linkedin.com/in/naveen-chandu-thupakula-853199275/)
- Email: naveenchandu200401@gmail.com

## 🙏 Acknowledgments

- Telugu Unicode Consortium for character standards
- OpenCV community for image processing tools
- TensorFlow/PyTorch teams for deep learning frameworks

## 📞 Contact

For any queries or suggestions, feel free to reach out:
- Email: naveenchandu200401@gmail.com
- LinkedIn: [Naveen Chandu Thupakula](https://www.linkedin.com/in/naveen-chandu-thupakula-853199275/)

---

⭐ If you found this project helpful, please consider giving it a star!
