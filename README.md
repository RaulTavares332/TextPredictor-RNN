# 🧠 TextPredictor-RNN  
**Character-Level Text Generation using Recurrent Neural Networks (RNN) and TensorFlow**

---

### 📘 Overview  
**TextPredictor-RNN** is a machine learning project designed to generate text **character by character**, learning linguistic patterns, rhythm, and writing styles from any textual dataset — such as *Shakespeare plays*, *literary works*, or *song lyrics*.  

The model leverages **Recurrent Neural Networks (RNN)** implemented with **TensorFlow/Keras** to predict the next character in a sequence, ultimately producing coherent and stylistically consistent text from an initial prompt.

---

### ⚙️ Technologies Used
- 🐍 **Python 3.12+**  
- 🧠 **TensorFlow / Keras**  
- 🔢 **NumPy**  
- 📊 **Pandas**  
- 📈 **Matplotlib**

---

### 🧩 Model Architecture  
The neural network is composed of the following layers:
1. **Embedding Layer** – Converts characters into dense numerical vectors  
2. **SimpleRNN Layer** – Captures sequential dependencies and temporal relationships between characters  
3. **Dense Output Layer** – Predicts the next most likely character in the sequence  

This architecture allows the model to understand complex text patterns and generate fluent, context-aware predictions.

---

### 🚀 Key Features
- 🔤 Trainable on any custom text corpus (e.g., `shakespeare.txt`, articles, song lyrics)  
- ✍️ Generates continuous, coherent text based on a user-provided seed phrase  
- 🎛️ Adjustable creativity level using the **temperature** parameter  
- 💾 Automatic **checkpoint saving** for model weights and training progress  
- 📚 Compatible with multiple languages and adaptable to different writing styles  

---

### 🧠 Example Usage
```python
print(generate_text(
    new_model,
    start_string="ROMEO: ",
    num_generate=300,
    temperature=1.0
))
