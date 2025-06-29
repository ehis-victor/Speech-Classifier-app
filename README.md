# 🗣️ Speech Classification Flask App

This project is a simple web application built with Flask that uses a pre-trained machine learning model to classify speech/text input. The app takes user input from a web form, processes it using a vectorizer and a model, and returns the prediction.

---

## ✨ Features

- Web interface for user input
- Text vectorization using a pre-trained CountVectorizer
- Speech/text classification using a pre-trained ML model
- JSON API endpoint for predictions

## 📁 Project Structure

```
Speechclf/
│
├── app.py
├── model.pkl
├── cv.pkl
├── requirements.txt
└── templates/
    └── index.html
```

## 📦 Requirements

All dependencies are listed in `requirements.txt`.  
To install them, run:

```
pip install -r requirements.txt
```

## 🚀 Usage

1. Make sure `model.pkl` and `cv.pkl` are present in the project directory.
2. Start the Flask app:

   ```
   python app.py
   ```

3. Open your browser and go to [http://127.0.0.1:5000/](http://127.0.0.1:5000/).
4. Enter your text in the form and submit to get a prediction.

## 🔗 API Endpoint

- **POST** `/predict`
  - Form data: `text` (string)
  - Returns: JSON with prediction

## 📝 Notes

- The model and vectorizer files (`model.pkl`, `cv.pkl`) must be generated and placed in the project directory.
- The web interface template should be in the `templates` folder as `index.html`.

## 📄 License

This project is for educational purposes.
