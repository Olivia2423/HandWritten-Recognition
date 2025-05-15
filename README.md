# Handwritten Digit Recognition


## 🎥 Demo Video

[▶️ Watch the Demo Video on Google Drive](https://drive.google.com/file/d/1opwUXqruQPWdrxatOmHbkEPsyE5yPplS/view?usp=sharing)

This project uses a neural network built with TensorFlow to recognize handwritten digits.  
Feed images of your own digits (PNG) into the **`digits/`** folder and the model will predict each digit.

---

##  Features
- Pre‑trained on the MNIST dataset  
- Loads model from **`handwritten.keras`** and predicts digits 0‑9  
- Resizes and normalizes any input image to 28 × 28 grayscale  
- Displays each prediction with a 1‑second preview (`matplotlib`)  
- Simple, lightweight fully‑connected architecture (2 × 128‑unit hidden layers)  

---

##  Model Architecture

```python
model = tf.keras.models.Sequential([
    tf.keras.layers.Flatten(input_shape=(28, 28)),
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dense(10, activation='softmax')
])
````

##  Setup

### 1. Clone

```bash
git clone https://github.com/yourusername/handwritten-digit-recognition.git
cd handwritten-digit-recognition
```

### 2. Install dependencies
```bash
pip install tensorflow opencv-python numpy matplotlib
```

### 3. Add images
```bash
Place PNG files in the digits/ folder with names like
```

### 4. Run
```bash
python main.py
```
