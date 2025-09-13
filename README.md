# 🎥 Automatic Attendance Manager

A Python-based **facial recognition attendance system** that uses real-time webcam feed to detect and recognize faces, and automatically logs attendance into a CSV file with timestamps.

---

## ✨ Features

- ✅ Face detection & recognition using **dlib’s ResNet model** (via `face_recognition` library).  
- ✅ Real-time video processing with **OpenCV**.  
- ✅ Maintain a directory of known faces (`knownfaces/`) for recognition.  
- ✅ Automatically logs attendance in **CSV format** (`attendance.csv`) with name and timestamp.  
- ✅ Prevents duplicate entries for the same person.  
- ✅ Easy to extend and integrate into other systems.

---

## 🛠 Tech Stack

- **Python 3.x**
- **OpenCV** – real-time video capture & display  
- **face_recognition** – face detection & encoding  
- **NumPy** – numerical operations  
- **CSV Logging** – attendance records stored as `Name, Time`

---

## 📂 Project Structure

Automatic-Attendance-Manager/
├── attandance.py # Main script to run attendance system
├── attendance.csv # CSV file storing attendance logs
├── knownfaces/ # Folder containing images of known individuals
├── README.md # Project documentation


---

## 🚀 Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/SandipanSom/Automatic-Attendance-Manager.git
cd Automatic-Attendance-Manager
2️⃣ Install dependencies
pip install opencv-python face-recognition numpy

3️⃣ Add known faces

Place images (.jpg, .jpeg, .png) of people you want to recognize inside the knownfaces/ directory.

The filename (without extension) will be used as the person’s name.

Example:

knownfaces/
 ├── Alice.jpg
 ├── Bob.png
 └── Charlie.jpeg

4️⃣ Run the program
python attandance.py


Press q to exit the webcam window.

📝 Usage

Launch the script → webcam starts.

If a face matches someone from knownfaces/, their name and timestamp are logged into attendance.csv.

If no match is found, the face is labeled as Unknown (not logged).

Sample attendance.csv output:

Name,Time
Alice,2025-09-14 09:15:23
Bob,2025-09-14 09:18:47

👤 Author

Sandipan Som
