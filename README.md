# Distance Real-Time Prediction

A real-time distance prediction application with GPS tracking and data visualization.

## Prerequisites

- Python 3.10 or higher
- Git
- pip (comes with Python)

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/MalikTolegen/Distance-Real-Time-Prediction.git
cd Distance-Real-Time-Prediction
```

### 2. Create a Virtual Environment

```bash
# On Windows
python -m venv .venv

# On macOS/Linux
python3 -m venv .venv
```

### 3. Activate the Virtual Environment

**Windows:**
```bash
.venv\Scripts\activate
```

**macOS/Linux:**
```bash
source .venv/bin/activate
```

You should see `(.venv)` at the beginning of your terminal prompt when activated.

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

This will install:
- pyserial
- numpy
- pyqtgraph
- PyQt5
- scipy

### 5. Run the Application

```bash
python main.py
```

The application will start and display the main window with real-time data visualization and distance prediction features.

## Project Structure

```
.
├── main.py                 # Main application entry point
├── MainWindow.py           # GUI window implementation
├── ViewModel.py            # View model for data handling
├── CommWorker.py           # Serial communication worker
├── GpsWorker.py            # GPS data processing worker
├── DistanceCalculator.py   # Distance calculation logic
├── Protocol.py             # Communication protocol definitions
├── requirements.txt        # Python dependencies
└── README.md               # This file
```

## Deactivating the Virtual Environment

When you're done, deactivate the virtual environment:

```bash
deactivate
```

## Troubleshooting

### Virtual Environment Won't Activate
- Ensure you're in the correct directory containing the `.venv` folder
- Try deleting `.venv` and recreating it: `python -m venv .venv`

### Module Import Errors
- Verify the virtual environment is activated (check for `(.venv)` in your terminal)
- Reinstall dependencies: `pip install -r requirements.txt`

### Serial/GPS Connection Issues
- Check that your device is properly connected
- Verify the correct COM port is configured
- Ensure PySerial is installed correctly: `pip install pyserial`

## License

This project is created by Malik Tolegen.
