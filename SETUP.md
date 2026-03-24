# Setup Instructions

## Folder Structure
Your project should have the following structure:

```
Food-Detection-using-CNN/
├── data/
│   ├── train/
│   │   ├── burger/       (put burger images here)
│   │   ├── masala_dosa/  (put masala dosa images here)
│   │   ├── momos/        (put momos images here)
│   │   ├── pizza/        (put pizza images here)
│   │   └── samosa/       (put samosa images here)
│   └── Metafile1.csv     (move your metadata CSV here)
├── models/               (trained models will be saved here)
├── .env                  (your environment variables - DO NOT commit this)
├── .env.example          (template for environment variables)
├── tensorflow.ipynb      (main notebook)
└── README.md
```

## Steps to Get Started

### 1. Move Your Training Data
Copy your images from:
- `C:\Users\aarus\Desktop\pt train\train\*`

To:
- `data/train/burger/`
- `data/train/masala_dosa/`
- `data/train/momos/`
- `data/train/pizza/`
- `data/train/samosa/`

### 2. Move Your Metadata File
Copy `C:\Users\aarus\Desktop\Metafile1.csv` to:
- `data/Metafile1.csv`

### 3. Setup Environment Variables
1. Copy `.env.example` to `.env`
2. Add your ngrok auth token:
   ```
   NGROK_AUTH_TOKEN=your_actual_token_here
   ```

### 4. Run the Notebook
Now you can run the notebook and all paths will work correctly!

## Note
The `data/` and `models/` directories are in `.gitignore`, so your large files won't be uploaded to GitHub.
