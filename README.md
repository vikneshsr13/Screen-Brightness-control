Screen Brightness Control Using Python

This project dynamically adjusts the screen brightness based on ambient lighting conditions captured through a webcam. It uses Python for the implementation and leverages computer vision techniques to estimate light levels.
Features
- Detects ambient light using a webcam.
- Dynamically adjusts screen brightness for optimal visibility and reduced eye strain.
- Works across various lighting conditions.
- Customizable brightness thresholds.

Prerequisites
Make sure you have the following installed on your system:
- Python 3.x
- `opencv-python` for capturing and processing webcam input
- `numpy` for image processing
- `screen-brightness-control` (optional, for controlling screen brightness on supported systems)

Install the required libraries using pip:
```bash
pip install opencv-python numpy screen-brightness-control
```

How It Works
1. The webcam captures frames of the environment.
2. Each frame is converted to grayscale, and the average pixel intensity is calculated to determine the ambient light level.
3. Based on the calculated brightness, the screen brightness is adjusted using the `screen-brightness-control` library.

Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/screen-brightness-control.git
   cd screen-brightness-control
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the program:
   ```bash
   python brightness_control.py
   ```

Usage
- Ensure the webcam is enabled and functioning.
- The script will automatically adjust the brightness in real time.
- You can customize the brightness thresholds in the script.

Project Structure
```
screen-brightness-control/
├── brightness_control.py  # Main script for brightness control
├── README.md              # Project documentation
├── requirements.txt       # List of dependencies
```

 Customization
- Adjust brightness thresholds or calibration settings in the script (`brightness_control.py`) to suit your needs.
- Modify the frame processing logic to filter out unnecessary light sources.

 Limitations
- The accuracy of brightness adjustment depends on the quality of the webcam.
- External factors, like rapidly changing light conditions, may affect performance.
- Limited compatibility for screen brightness control on certain operating systems.

Future Enhancements
- Add face detection to focus brightness adjustment on ambient light, excluding screen reflections.
- Implement machine learning to better classify and respond to complex lighting conditions.
- Add support for multi-monitor setups.

 License
This project is licensed under the MIT License. See the `LICENSE` file for details.

 Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request.


 Author
(https://github.com/vikneshsr13)  
