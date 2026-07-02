# Rule-Based Medical FAQ Chatbot — Blood Pressure

Medical FAQ chatbot specialised in blood pressure and hypertension questions, built with intent classification and a neural network classifier.

## How it works

1. **Text preprocessing** — NLTK tokenization, lemmatization, bag-of-words encoding
2. **Intent classifier** — 3-layer Keras neural network trained on categorised Q&A pairs
3. **Response selection** — probabilistic intent matching with a confidence threshold; falls back to a default reply below threshold

## Intent categories (intents.json)

Blood pressure causes, normal vs high readings, hypertension symptoms, medication types, lifestyle interventions (diet, exercise, stress), emergency warning signs, and general health advice.

## Files

| File | Description |
|---|---|
| `ChatBot_BlodPressure.ipynb` | Training notebook: preprocessing, model definition, training loop, inference demo |
| `train_chatbot.py` | Standalone training script |
| `chatgui.py` | Tkinter GUI for interactive chat |
| `intents.json` | Intent dataset: patterns and responses |
| `chatbot_model.h5` | Trained Keras model |

## Stack

NLTK · TensorFlow/Keras · NumPy · pickle · Tkinter
