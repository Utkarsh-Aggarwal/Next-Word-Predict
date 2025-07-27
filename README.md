🚀 Next Word Predictor (LSTM)
This is a deep learning-based Next Word Prediction model trained using an LSTM neural network. It uses a preprocessed text corpus to predict the most likely next word based on the input sequence. The model is deployed using Gradio on Hugging Face Spaces for an interactive demo.

🔗 Live Demo:
[👉 Try it here](https://huggingface.co/spaces/UtkarshAggarwal234/NEXT-Word)

🧠 How it Works
The model is trained on a corpus using a tokenizer that converts text into sequences.

It uses an LSTM (Long Short-Term Memory) neural network to learn patterns in the text.

Given a user input (partial sentence), it predicts the most likely next word.

📁 Project Structure
NEXT-Word/
├── app.py                   # Gradio interface and prediction logic
├── requirements.txt         # Dependencies for Hugging Face Spaces
├── tokenizer.pickle         # Saved tokenizer used during training
└── next_word_lstm_model.h5  # Trained LSTM model

📦 Requirements
The dependencies are handled automatically on Hugging Face Spaces via requirements.txt. If running locally, you can install them with:

pip install -r requirements.txt

▶️ Running Locally
python app.py
This will launch a Gradio interface in your browser where you can test the next word predictions interactively.

📚 Example
Input:
The quick brown

Predicted Next Word:
fox

📌 Notes
The tokenizer must match the one used during training.

The LSTM model expects input of fixed sequence length.

Only the most probable word is returned, but the model can be extended to return the top-k words with probabilities.
