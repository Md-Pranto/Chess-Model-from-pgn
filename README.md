# Chess Neural Network (2400+ Rated Games)

This project trains a neural network to predict and play chess moves based on professional-level games. It leverages high-rated Lichess data to build a model capable of making strategic decisions and playing real games.

---

## Overview

* Collected **PGN data** from [Lichess](https://database.nikonoel.fr/)
* Filtered matches played between **2400+ rated players** for high-quality strategies
* Built and trained a **3-layer Neural Network** using TensorFlow/Keras
* Trained **`.keras` model** can evaluate positions and play real games

---

## Model Architecture

* **Input:** Encoded chess board `(8×8×12)`
* **Layers:**

  * `Conv2D(64, (3,3), activation='relu')`
  * `Conv2D(128, (3,3), activation='relu')`
  * `Flatten()`
  * `Dense(256, activation='relu')`
  * `Dense(output_size, activation='softmax')`
* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy

---

## Features

* Uses **high-level professional data** for training
* Predicts **legal chess moves** using model outputs
* Compatible with **chess engines or UIs** (e.g., `python-chess`)
* Can be used for **real-time chess gameplay**

---

## 📂 Project Structure

```
Chess-NN/
│
├─ data/               # PGN files and preprocessed data
├─ models/             # Trained .keras model files
├─ notebooks/          # Jupyter notebooks for training and analysis
├─ src/                # Python scripts for training and gameplay
└─ README.md
```

---

## Usage

1. **Install dependencies**:

```bash
pip install tensorflow numpy python-chess
```

2. **Load model and play**:

```python
from tensorflow.keras.models import load_model
import chess

model = load_model("models/mymodel_100epoch_9k.keras")
# Use your gameplay script to make moves based on model predictions
```

---

## Future Improvements

* Add **reinforcement learning** via self-play
* Implement **MCTS (Monte Carlo Tree Search)** for deeper evaluation
* Train on **larger datasets** to reach grandmaster-level performance
* Optimize for **faster inference** and **GPU parallelism**

---

## License

This project is licensed under the **MIT License**. Feel free to use and modify it for research or personal projects.

---

## References

* [Lichess PGN Data](https://database.nikonoel.fr/)(Chess Neural Network (2400+ Rated Games)

This project trains a neural network to predict and play chess moves based on professional-level games. It leverages high-rated Lichess data to build a model capable of making strategic decisions and playing real games.

---

## Overview

* Collected **PGN data** from [Lichess](https://lichess.org/)
* Filtered matches played between **2400+ rated players** for high-quality strategies
* Built and trained a **3-layer Neural Network** using TensorFlow/Keras
* Trained **`.keras` model** can evaluate positions and play real games

---

## Model Architecture

* **Input:** Encoded chess board `(8×8×12)`
* **Layers:**

  * `Conv2D(64, (3,3), activation='relu')`
  * `Conv2D(128, (3,3), activation='relu')`
  * `Flatten()`
  * `Dense(256, activation='relu')`
  * `Dense(output_size, activation='softmax')`
* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy

---

## Features

* Uses **high-level professional data** for training
* Predicts **legal chess moves** using model outputs
* Compatible with **chess engines or UIs** (e.g., `python-chess`)
* Can be used for **real-time chess gameplay**

---

## Usage

1. **Install dependencies**:

```bash
pip install tensorflow numpy python-chess
```

2. **Load model and play**:

```python
from tensorflow.keras.models import load_model
import chess

model = load_model("models/mymodel_100epoch_9k.keras")
# Use your gameplay script to make moves based on model predictions
```

---

## Future Improvements

* Add **reinforcement learning** via self-play
* Implement **MCTS (Monte Carlo Tree Search)** for deeper evaluation
* Train on **larger datasets** to reach grandmaster-level performance
* Optimize for **faster inference** and **GPU parallelism**

---

## License

This project is licensed under the **MIT License**. Feel free to use and modify it for research or personal projects.

---

## References

* [Lichess PGN Data](https://database.nikonoel.fr/)
* [TensorFlow Documentation](https://www.tensorflow.org/)
* [Python-Chess Library](https://python-chess.readthedocs.io/)

---

**Model File:** `models/mymodel_100epoch_9k.keras`
**Framework:** TensorFlow / Keras
**Dataset Source:** Lichess PGN archives
)
* [TensorFlow Documentation](https://www.tensorflow.org/)
* [Python-Chess Library](https://python-chess.readthedocs.io/)

---

**Model File:** `models/mymodel_100epoch_9k.keras`
**Framework:** TensorFlow / Keras
**Dataset Source:** Lichess PGN archives
