
# ⚙️ Installation and Usage Guide

Follow these steps to set up and run the **Heart Disease Predictor** project on your local machine.

---

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/heart-disease-predictor.git
cd heart-disease-predictor
```

---

## 2. Create and Activate a Virtual Environment

### 🔹 Create the Environment

```bash
python -m venv venv
```

### 🔹 Activate the Environment

- **Windows:**

  ```bash
  venv\Scripts\activate
  ```

- **Linux/macOS:**

  ```bash
  source venv/bin/activate
  ```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Register the Environment with Jupyter

```bash
pip install ipykernel
python -m ipykernel install --user --name=heart-disease-env --display-name "Heart Disease Env"
```

This will make your virtual environment available as a Jupyter kernel.

---

## 5. Launch Jupyter Lab

```bash
jupyter lab
```

Then, open the notebook file:

```bash
Predictive Diagnostics.ipynb
```

✅ Make sure the selected kernel is **Heart Disease Env**.

---

You're now ready to run the prediction section and use the **Heart Disease Predictor**!
