## # ⚙️ Installation and Usage Guide
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/heart-disease-predictor.git
cd heart-disease-predictor
```
### 2.Create a Virtual Enviornment
```bash
python -m venv venv
```
Activate the Enviornement
* Windows
```bash
venv\Scripts\activate
```
*Linux\macOS
```bash
source venv/bin/activate
```

### 3.Install Dependencies
```bash
pip install -r requirements.txt
```
### 4.Register The Enviornement with Jupyter
```bash
pip install ipykernel
python -m ipykernel install --user --name=heart-disease-env --display-name "Heart Disease Env"
```
### 5.Launch Jupyter Lab
```bash
jupyter lab
```
Open the Notebok file with extendion .ipynb
```ngnix
Predictive Diagnostics.ipynb
```
make sure the Kernal selected is Heart Disease env
