# BRAU_NewB-ew_Hackerthon_KUET_2024
# Bengali Transliteration API

This repository provides a Flask-based backend and a React-based frontend for a Bengali transliteration model. The backend is designed to preprocess input data and serve predictions using a fine-tuned model.

## Features
- **Backend:** Flask application to serve predictions via an API endpoint.
- **Frontend:** React application for user interaction.
- **Model:** Fine-tuned `google/mt5-small` transformer model.

## Prerequisites
Before running the application, ensure the following are installed:

- Python 3.8+
- Node.js 16+
- Git

## Folder Structure
```
project/
├── app.py                # Flask backend
├── requirements.txt      # Python dependencies
├── .gitignore            # Ignored files
├── README.md             # Documentation (this file)
├── frontend/             # React frontend code
├── model/                # (Optional) Pretrained model files
```

## Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-folder>
```

### 2. Backend Setup

#### Install Dependencies
```bash
pip install -r requirements.txt
```

#### Run Flask Application
```bash
python app.py
```
The backend will be available at `http://127.0.0.1:5000/`.

### 3. Frontend Setup

#### Install Dependencies
Navigate to the `frontend/` folder and run:
```bash
npm install
```

#### Start the React Application
```bash
npm start
```
The frontend will be available at `http://localhost:3000/`.

## API Endpoints

### POST `/predict`
**Description:** Transliterates input text from Banglish (Romanized Bengali) to Bengali.

**Request Body:**
```json
{
  "text": "eta kono post holo mia abal"
}
```

**Response:**
```json
{
  "transliteration": "এটা কোনো পোস্ট হলো মিয়া আবাল"
}
```

## Future Work
- Train the model further for improved accuracy.
- Add more language support.
- Enhance the frontend design.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any suggestions or improvements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
