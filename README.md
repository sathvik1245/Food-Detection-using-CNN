# Food Detection using CNN

A Convolutional Neural Network (CNN) model to classify food images into 5 categories: burger, masala_dosa, momos, pizza, and samosa.

## Features

- CNN-based image classification
- Web interface for real-time predictions
- Flask API with drag-and-drop image upload
- Ngrok integration for public access

## Setup

### Prerequisites

- Python 3.8+
- TensorFlow
- Flask
- Other dependencies (see requirements.txt)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/Food-Detection-using-CNN.git
cd Food-Detection-using-CNN
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your environment variables:
```bash
cp .env.example .env
# Edit .env and add your NGROK_AUTH_TOKEN
```

4. Prepare your data:
   - Place training images in `data/train/` with subfolders for each class
   - Place your metadata CSV in `data/Metafile1.csv`

### Project Structure

```
Food-Detection-using-CNN/
├── data/
│   ├── train/           # Training images by category
│   └── Metafile1.csv    # Metadata file
├── models/              # Saved model files
├── tensorflow.ipynb     # Main notebook
├── .env.example         # Environment variables template
├── .gitignore
└── README.md
```

## Usage

### Training the Model

Open and run `tensorflow.ipynb` to:
1. Load and preprocess images
2. Build and train the CNN model
3. Save the trained model

### Running the Web App

Run the Flask application from the notebook or:
```python
python app.py  # If you extract the Flask app to a separate file
```

The web interface will be available at `http://localhost:5000` or via ngrok public URL.

## Model Architecture

- Input: 30x30x3 RGB images
- 3 Convolutional layers with MaxPooling
- Dense layers with softmax activation
- 5 output classes

## Food Categories

1. Burger
2. Masala Dosa
3. Momos
4. Pizza
5. Samosa

## License

MIT License

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.