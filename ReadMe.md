# Facial Presence Ledger

A facial recognition-based attendance tracking system that automatically identifies and logs the presence of authorized personnel using computer vision and deep learning technologies.

## Features

- **Facial Recognition**: Uses VGGFace model for accurate face detection and recognition
- **Automated Attendance**: Automatically logs attendance when authorized faces are detected
- **CSV Database**: Stores attendance records with name, date, subject, and session information
- **Pre-trained Models**: Utilizes pre-trained deep learning models for reliable facial recognition
- **Real-time Processing**: Processes video input in real-time using OpenCV

## Technology Stack

- **Deep Learning**: TensorFlow and Keras for neural network operations
- **Computer Vision**: OpenCV for image and video processing
- **Facial Recognition**: DeepFace library for face analysis
- **Data Management**: Pandas for data manipulation and CSV handling
- **Numerical Computing**: NumPy for mathematical operations

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/omairakapasha/Facial-Presence-Ledger.git
   cd Facial-Presence-Ledger
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Verify installation**
   ```bash
   python -c "import cv2, deepface, tensorflow; print('All dependencies installed successfully')"
   ```

## Project Structure

```
Facial-Presence-Ledger/
├── Authorized_Personals/          # Pre-trained models and authorized person data
│   └── ds_model_vggface_...pkl    # VGGFace detector model
├── Database/                      # Attendance records storage
│   └── attendance.csv            # CSV file with attendance logs
├── Model                         # Core application logic (to be implemented)
├── requirements.txt              # Python dependencies
├── LICENSE                       # CC0 1.0 Universal License
└── ReadMe.md                    # Project documentation
```

## Dependencies

| Package | Version | Purpose |
|---------|---------|---------|
| deepface | 0.0.93 | Facial recognition and analysis |
| opencv-python | 4.11.0.86 | Computer vision and image processing |
| pandas | 2.3.0 | Data manipulation and CSV handling |
| tensorflow | 2.16.2 | Deep learning framework |
| tf-keras | 2.16.0 | High-level neural networks API |
| numpy | 1.26.4 | Numerical computing |

## Usage

> **Note**: The core application logic is currently under development. The following represents the intended functionality.

### Basic Usage

1. **Initialize the system**
   ```bash
   python main.py
   ```

2. **Add authorized personnel**
   - Place reference images in the `Authorized_Personals/` directory
   - The system will create facial encodings for recognition

3. **Start attendance tracking**
   - Point your camera towards the area to monitor
   - The system will automatically detect and log attendance

### Attendance Data

Attendance records are stored in `Database/attendance.csv` with the following structure:
- **Name**: Identified person's name
- **Date**: Date of attendance
- **Subject**: Subject or event being tracked
- **Session**: Session identifier

## Development Status

This project is currently in the initial development phase. The following components are planned:

- [ ] Core facial recognition engine
- [ ] Real-time video processing
- [ ] GUI interface
- [ ] Database management system
- [ ] Configuration management
- [ ] Batch processing capabilities
- [ ] Reporting and analytics

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for:

- Bug fixes
- Feature enhancements
- Documentation improvements
- Performance optimizations

## License

This project is licensed under the CC0 1.0 Universal License - see the [LICENSE](LICENSE) file for details. This means the work is in the public domain and you can copy, modify, and distribute it without restrictions.

## Acknowledgments

- **DeepFace**: For providing robust facial recognition capabilities
- **OpenCV**: For computer vision functionality
- **TensorFlow**: For deep learning framework
- **VGGFace**: For the pre-trained facial recognition model

## Support

For questions, issues, or contributions, please visit the [GitHub repository](https://github.com/omairakapasha/Facial-Presence-Ledger) or open an issue.

---

*This project aims to provide an efficient and accurate solution for automated attendance tracking using modern computer vision techniques.*