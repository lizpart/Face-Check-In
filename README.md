# Face-Check-In

This Flask application is designed to automate attendance tracking using face recognition technology. It allows users to register their faces and then automatically mark their attendance when they appear in front of a camera.

# Features
 - Real-time Face Recognition: Utilizes OpenCV to capture video from a webcam and recognize faces in real-time.
 - Attendance Logging: Records attendance in a CSV file with the date and time stamp.
 - User Registration: Allows users to register their faces by capturing multiple images for training the face recognition model.
 - Dynamic Web Interface: Provides a user-friendly web interface for interaction.

# Prerequisites
 * Python 3.x
 * OpenCV (`pip install opencv-python`)
 * Flask (`pip install Flask`)
 * NumPy (`pip install numpy`)
 * Scikit-learn (`pip install scikit-learn`)
 * Pandas (`pip install pandas`)

# Setup Instructions
1. Clone the repository to your local machine.
2. Install the required Python packages using pip install -r requirements.txt.
3. Ensure that the necessary directories (Attendance and static/faces) exist. If not, create them manually.
4. Make sure the haarcascade_frontalface_default.xml file is located in the specified directory (static).
5. Run the Flask app using python app.py.
6. Access the app via your web browser at http://localhost:5000.

# Dependencies
 - OpenCV (`cv2`) for face detection and image processing.
 - Flask for creating the web application.
 - NumPy and pandas for data manipulation.
 - scikit-learn for machine learning tasks such as training the K Nearest Neighbors classifier.

# File Structure
 - app.py: Flask application containing routing functions and main functionality.
 - static: Directory containing static files such as CSS, JavaScript, and XML files.
 - haarcascade_frontalface_default.xml: XML file used for face detection.
 - templates: Directory containing HTML templates for rendering web pages.

# Usage
1. Visit the main page of the web application.
2. View the attendance records for the current date.
3. Click on "Take Attendance" to start capturing faces and mark attendance automatically.
4. Click on "Add New User" to add a new user to the system by capturing their face images.

# Note
Ensure that the webcam is properly connected and accessible by the application.
Train the face recognition model before using the system by capturing images of registered users.
