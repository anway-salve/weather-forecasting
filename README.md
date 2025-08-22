# 🌦️ Weather Prediction using Time Series Analysis  

This project predicts precipitation (rainfall) in inches based on historical weather attributes using **Linear Regression**. Two different user interfaces are provided:  

1. **Streamlit Web App (`app.py`)** – Interactive browser-based UI.  
2. **Tkinter Desktop App (`weather.py`)** – GUI application for desktop use.  

---

## 📂 Project Structure  

```
├── app.py              # Streamlit-based weather prediction web app
├── weather.py          # Tkinter-based weather prediction desktop app
├── austin_final_final.csv   # Dataset (must be placed in project folder)
```

---

## ⚙️ Requirements  

Install dependencies before running:  

```bash
pip install streamlit pandas numpy scikit-learn matplotlib
```

For Tkinter (usually pre-installed with Python):  
```bash
sudo apt-get install python3-tk   # (Linux)
```

---

## 🚀 Running the Applications  

### 1. Streamlit App (`app.py`)  
Run in terminal:  
```bash
streamlit run app.py
```

Then open the link (usually `http://localhost:8501/`) in your browser.  

Features:  
- Enter weather attributes (temperature, dew point, humidity, pressure, visibility, wind).  
- Predict precipitation (in inches).  
- Displays rainfall expectation:  
  - 🌧️ High  
  - 🌦️ Moderate  
  - 🌤️ Low  
- Graphs:  
  - Precipitation over time.  
  - Trends of selected weather attributes.  

---

### 2. Tkinter App (`weather.py`)  
Run in terminal:  
```bash
python weather.py
```

Features:  
- Desktop GUI form to enter weather attributes.  
- Predicts precipitation.  
- Displays rainfall category (High, Moderate, Low).  
- Plots precipitation trends and feature-wise graphs.  

---

## 📊 Dataset  

The model uses **`austin_final_final.csv`**, a cleaned Austin weather dataset.  
- Input features:  
  - Temperature (High/Avg/Low), Dew Point, Humidity, Sea Level Pressure, Visibility, Wind Speed.  
- Output label:  
  - `PrecipitationSumInches`  

---

## 🔮 Model  

- **Algorithm**: Linear Regression (`sklearn.linear_model.LinearRegression`)  
- **Training**:  
  - `X`: Weather attributes  
  - `Y`: Precipitation (reshaped into 2D vector)  
- Predictions are based on real-time user input.  

---

## 📌 Notes  

- Both apps require the dataset file (`austin_final_final.csv`) in the **same directory**.  
- Streamlit app is recommended for web-based use.  
- Tkinter app is useful for offline desktop usage.  

---

✅ With these applications, you can explore how weather attributes influence precipitation and visualize trends interactively.  
