# AI-Based Intruder Detection System

An intelligent real-time surveillance system that detects and alerts when unknown individuals appear on camera. The system uses computer vision and facial recognition to identify authorized personnel and triggers alarms for unauthorized access.

## 🎯 Key Features

- **Real-time Face Detection**: Continuously monitors camera feed using OpenCV for instant detection
- **Database-Driven Recognition**: Compares detected faces against a database of authorized personnel
- **Intelligent Alarm System**: Automatically triggers alerts when unknown individuals are detected
- **Visual Feedback**: Displays bounding boxes around detected persons for clear identification
- **Performance Optimized**: Implements frame throttling and FPS optimization for efficient processing

## 🛠️ Technical Stack

- **OpenCV**: Computer vision and image processing
- **Python**: Core programming language
- **Face Recognition Library**: For encoding and comparing facial features
- **Database**: Stores authorized personnel face encodings

## 🚀 How It Works

1. **Face Detection**: The system continuously captures frames from the camera feed and detects faces using OpenCV's Haar Cascades or deep learning models
2. **Face Recognition**: Detected faces are encoded and compared against the database of known individuals
3. **Decision Making**: If a face doesn't match any stored encoding, it's classified as an intruder
4. **Alert Triggering**: An alarm is immediately triggered when an unauthorized person is detected
5. **Visual Indication**: Rounded bounding boxes are drawn around detected persons for monitoring

## ⚡ Performance Optimizations

- **Frame Throttling**: Processes every Nth frame to reduce computational load while maintaining detection accuracy
- **FPS Management**: Optimizes frame processing rate to balance between detection speed and system resources
- **Efficient Encoding**: Pre-computed face encodings stored in database for faster comparison
- **Multi-threading**: Separates video capture, processing, and alarm triggering into different threads

## 📋 Prerequisites

```bash
Python 3.7+
OpenCV (cv2)
face_recognition
numpy
```

## 🔧 Installation

```bash
# Clone the repository
git clone <repository-url>
cd intruder-detection-system

# Install required packages
pip install opencv-python face_recognition numpy

# Set up the database with authorized personnel images
python setup_database.py
```

## 💻 Usage

```bash
# Run the detection system
python main.py

# Add new authorized personnel
python add_person.py --name "John Doe" --image "path/to/image.jpg"
```

## 🎨 Features in Detail

### Face Database Management
- Add, update, and remove authorized personnel
- Supports multiple images per person for better recognition accuracy
- Efficient storage of face encodings

### Alarm System
- Customizable alarm sounds
- Adjustable sensitivity and trigger delay
- Log system for tracking detection events

### Visual Interface
- Real-time camera feed display
- Color-coded bounding boxes (green for authorized, red for intruders)
- FPS counter and system status indicators

## 🔒 Security Considerations

- Face encodings are stored securely in the database
- System can be configured to log all detection events
- Option to capture and store images of detected intruders
- Integration-ready with external security systems

## 📊 Performance Metrics

- Detection accuracy: High precision with proper database setup
- Processing speed: Optimized for real-time performance
- Resource usage: Minimal CPU/GPU load through intelligent throttling

## 🔮 Future Enhancements

- Multi-camera support
- Cloud-based database synchronization
- Mobile app notifications
- Advanced analytics and reporting dashboard
- Integration with access control systems


## 👨‍💻 Author

[Vikas Mishra]



