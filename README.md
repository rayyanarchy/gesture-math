# Hand Gesture Math Operations

Hand Gesture Math Operations is a web-based application that performs basic math operations (addition and subtraction) using hand gestures. It uses your webcam to capture hand gesture images representing numbers, processes them to determine the operation, and displays the result on the page.

## Preview

<p align="center">
  <img src="https://github.com/user-attachments/assets/7ffceecb-1568-431e-8d1c-e9493d4cd88a" alt="Homepage" width="70%">
</p>

## Features

- **Start Camera**: Activates the webcam to capture live video.
- **Capture Images**: Allows users to take snapshots of hand gestures for input.
- **Process Images**: Performs mathematical operations based on the captured images.
- **Results Display**: Shows the result of the operation on the web page.

## Prerequisites

- Python 3.9+
- [uv](https://docs.astral.sh/uv/) (recommended) or `pip`
- A webcam

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/rayyanarchy/gesture-math.git
   cd gesture-math
   ```

2. **Install dependencies**

   Using `uv` (recommended — creates the virtual environment and installs everything from `pyproject.toml` in one step):

   ```bash
   uv sync
   ```

   Or with plain `pip`:

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   pip install Flask mediapipe numpy
   ```

3. **Run the application**

   ```bash
   flask --app app/main run
   ```

   The application will be accessible at `http://127.0.0.1:5000`.

## How To Use

1. **Open the homepage** in your browser.
2. **Start the camera** — click "Start Camera" to activate the webcam and begin capturing live video.

   <p align="center">
     <img src="https://github.com/user-attachments/assets/64d1b91b-e8b7-4fbf-bb44-fdbfcad33080" alt="Start Camera" width="60%">
   </p>

3. **Capture hand gestures**
   - Click "Capture First Image" to take a snapshot of the first hand gesture.
   - Click "Capture Second Image" to take a snapshot of the second hand gesture.

   <p align="center">
     <img src="https://github.com/user-attachments/assets/aa78d991-af5a-4ee3-a620-6677daaca9de" alt="Capture first gesture" width="45%">
     <img src="https://github.com/user-attachments/assets/d1c878de-cbbc-4bf8-ad70-f8e85e13c535" alt="Capture second gesture" width="45%">
   </p>

4. **Select an operation** from the dropdown menu — "Add" or "Subtract".
5. **Process the images** — click "Process Images" to perform the selected operation based on the number of fingers shown.
6. **View the result**, displayed below the captured images.

   <p align="center">
     <img src="https://github.com/user-attachments/assets/a058f0aa-69d5-4382-a63e-8695f80e90ee" alt="Result" width="60%">
   </p>

## License

This project is open source and available under the [MIT License](LICENSE).
