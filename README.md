# 🚗🚧 Parking Spot Detection and Monitoring

This repository provides a comprehensive solution for detecting and monitoring parking spot occupancy in real-time using image processing and computer vision techniques. The system identifies parking spots, tracks their status, and displays available spaces dynamically.

## 🔄 Project Overview
The objective of this project is to utilize video streams and a pre-defined mask to classify parking spots as occupied or vacant. The implementation leverages OpenCV for image processing, connected components analysis for parking spot detection, and efficient frame differencing for occupancy classification. This tool is ideal for automating parking management and providing real-time data on parking availability.

## 🔧 Features
- **🌟 Parking Spot Detection**: Identifies parking spots using connected components and a mask.
- **⏳ Real-Time Status Monitoring**: Classifies spots as occupied or vacant based on frame differencing.
- **🎨 Dynamic Visualization**: Overlays bounding boxes and displays the number of available spots on the video feed.
- **⚙️ Efficient Processing**: Processes video frames in steps for optimized performance.

## 📂 Repository Contents
- **`main.py`**: Core script for detecting and monitoring parking spots.
- **`util.py`**: Utility functions for spot detection and classification.
- **`mask_1920_1080.png`**: Pre-defined mask for identifying parking spots.
- **`samples/`**: Directory containing sample video files (e.g., `parking_1920_1080_loop.mp4`).
- **`requirements.txt`**: List of required Python libraries.

## 🔄 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ArianDilfanian/parkingSpotDetectionAndCounter.git
   cd parkingSpotDetectionAndCounter

   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have the necessary input files:
   - A mask file for parking spot detection (e.g., `mask_1920_1080.png`).
   - A video file to analyze (e.g., `samples/parking_1920_1080_loop.mp4`).

## 🕹️ Usage
1. Run the script:
   ```bash
   python main.py
   ```

2. The program will process the video specified in `video_path` and display:
   - Detected parking spots with bounding boxes (🟢 green for vacant, 🔴 red for occupied).
   - A counter showing the number of available spots.

3. Press **'q'** to quit the visualization.

## 🔁 Customization
- **🛠️ Mask File**: Replace `mask_1920_1080.png` with a custom mask file for your parking layout.
- **🎥 Video File**: Modify `video_path` to use your own video feed.
- **⏳ Step Size**: Adjust the `step` variable for faster or slower frame processing.
- **🔢 Threshold**: Modify the criteria for classifying spots as vacant in `empty_or_not` or `calc_diff` functions.

## 🔬 How It Works
1. **🏦 Parking Spot Detection**: The pre-defined mask is analyzed using connected components to identify individual parking spots.
2. **⚔️ Frame Differencing**: Calculates differences between consecutive frames to detect changes in parking spot regions.
3. **🔹 Occupancy Classification**: Classifies spots as occupied or vacant based on calculated differences.
4. **🎨 Visualization**: Displays results dynamically with bounding boxes and an availability counter.

## ⚡️ Dependencies
- Python 3.8+
- OpenCV
- NumPy
- Matplotlib

Install these using:
```bash
pip install opencv-python-headless numpy matplotlib
```

## 💪 Contributing
Contributions are welcome! If you have suggestions, bug fixes, or new features, feel free to submit a pull request or open an issue.

## 🔒 License
This project is licensed under the [MIT License](LICENSE).

## 🌟 Acknowledgments
- [OpenCV](https://opencv.org/) for image processing tools.
- Inspiration from computer vision and smart parking systems.

---

## 🎥 Video



https://github.com/user-attachments/assets/5cccd1dc-d581-4808-aa94-ece72c5ba8ab
