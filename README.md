# Attendance System

This project is a Face Recognition-based Attendance System that uses OpenCV, face_recognition, and Pandas to recognize faces from a webcam and mark attendance in an Excel sheet (Attendance.xlsx).

Features
✅ Detects and recognizes faces in real time using a webcam
✅ Compares detected faces with known faces from an images/ folder
✅ Marks attendance in an Excel sheet (Attendance.xlsx) with a timestamp
✅ Uses face_recognition for accurate facial identification
✅ Draws bounding boxes around recognized faces

Installation
1️⃣ Clone the Repository
bash
Copy
git clone https://github.com/yourusername/face-recognition-attendance.git
cd face-recognition-attendance
2️⃣ Install Dependencies
Make sure you have Python 3.x installed, then install the required libraries:

bash
Copy
pip install opencv-python numpy face-recognition pandas openpyxl
3️⃣ Add Known Faces
Place images of known people inside the images/ folder
The file name (e.g., John_Doe.jpg) will be used as the person's name
Usage
Run the script to start the face recognition attendance system:

bash
Copy
python attendance.py
The webcam will open, detect faces, and mark attendance in Attendance.xlsx
Press Esc to exit the program
How It Works
1️⃣ Load known images: Reads images from the images/ folder and encodes them using face_recognition
2️⃣ Capture webcam frames: Reads video input and resizes frames for faster processing
3️⃣ Detect faces: Identifies faces and compares them with known encodings
4️⃣ Mark attendance: If a match is found, the person's name and timestamp are saved in Attendance.xlsx

File Structure
bash
Copy
📂 face-recognition-attendance  
 ├── 📂 images/              # Folder containing images of known faces  
 ├── 📝 Attendance.xlsx      # Excel file where attendance is recorded  
 ├── 📜 attendance.py        # Main script  
 ├── 📜 README.md            # Project documentation  
Requirements
Python 3.x
OpenCV (cv2)
face_recognition
NumPy
Pandas
OpenPyXL
Notes
The first time a face is recognized, it is added to the attendance sheet
The Excel file (Attendance.xlsx) is automatically created if it doesn’t exist
To improve accuracy, use high-quality, front-facing images in the images/ folder
Future Improvements
🔹 Add a GUI for better usability
🔹 Store attendance data in a database instead of an Excel file
🔹 Implement multi-face recognition in real-time

License
This project is open-source and free to use. Contributions are welcome! 🚀
