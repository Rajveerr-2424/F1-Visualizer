# 🏎️ F1 Fastest Lap Telemetry Visualization

A Python project that visualizes a Formula 1 driver’s **fastest lap** using real telemetry data from the **FastF1** library.  
This project generates a dark-themed, team-colored track map that highlights speed variations across the circuit and displays key lap insights such as **top speed** and **lap time**.

---

## 🚀 Features

- **Real F1 telemetry data** fetched using FastF1  
- **Fastest lap extraction** for any driver  
- **Team-themed color gradient** across the racing line  
- **Dark mode visualization** inspired by F1 broadcast graphics  
- **Accurate track layout** plotted from GPS (X/Y) telemetry  
- Displays **top speed** and **fastest lap time**  
- Automatically shows **Grand Prix name, location, and round**  

---

## 📂 Project Structure

```

F1-Telemetry-Visualizer/
│── main.py              # The main visualization script
│── README.md            # Project documentation
│── requirements.txt     # Required Python libraries
│── assets/              # (Optional) Saved plots or screenshots

```

---

## 🛠️ Technologies Used

- **Python 3**
- **FastF1**
- **Matplotlib**
- **NumPy**
- **LineCollection** (for gradient track coloring)

---

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/<your-username>/F1-Telemetry-Visualizer.git
cd F1-Telemetry-Visualizer
````

2. Install dependencies:

```bash
pip install fastf1 matplotlib numpy
```

---

## ▶️ Usage

Open `main.py` and edit the configuration at the top:

```python
year = 2023
wknd = 6
session_type = "R"
driver = "VER"
```

Then run:

```bash
python main.py
```

This will generate a full visualization of the driver’s fastest lap:

* Dynamic speed-color gradient
* Track path
* Top speed
* Lap time
* Grand Prix info

---

## 🧠 How It Works

* FastF1 loads the race session using:

  * Year
  * Weekend round number
  * Session type (Race, Qualifying, FP1, etc.)
* Telemetry is extracted from the driver’s **fastest lap**
* GPS coordinates (`X`, `Y`) plot the racing line
* Speed values generate a **team-themed gradient**
* Matplotlib displays the final styled visualization

---

## 🤝 Contributing

Pull requests and suggestions are welcome!
Feel free to fork the project and improve the visualization.

---

## 📜 License

This project is open-source under the **MIT License**.

---

## ⭐ Acknowledgements

* **FastF1** for access to official F1 timing data
* Matplotlib for the visualization tools

