# player-tracking-yolov8
🧰 Requirements

✅ Software & Environment
Python: 3.8 to 3.11
pip: Python package installer
OS: Windows / Linux / macOS
Hardware: GPU recommended (but works on CPU with lower speed)
📦 Dependencies

Install the following Python libraries:

pip install ultralytics opencv-python
If you also want CSV logging or advanced filtering:

pip install pandas
To optionally use Jupyter Notebooks (for exploration):

pip install jupyter
If you're using a virtual environment (recommended):

python -m venv venv
source venv/bin/activate       # Linux/macOS
venv\Scripts\activate.bat      # Windows

pip install -r requirements.txt
📄 requirements.txt (optional)

Create a file named requirements.txt with the following content:

ultralytics>=8.0.0
opencv-python
pandas
Then install everything via:

pip install -r requirements.txt
🔧 Folder Structure Example

player-tracking-yolov8/
├── player_tracking.py
├── best.pt                 # Your YOLOv8 trained model
├── video.mp4               # Input video
├── player_tracking_log.csv # (auto-created)
├── requirements.txt
├── README.md
▶️ How to Run the Code

Clone or download the repo:
git clone https://github.com/your-username/player-tracking-yolov8.git
cd player-tracking-yolov8
Place your trained YOLOv8 model (e.g. best.pt) in the project folder.
Place a test video (video.mp4) in the same folder.
Run the script:
python player_tracking.py
Press q to stop the video stream.
⚙️ Optional Configs

📹 Use Webcam Instead of Video
Edit this line in player_tracking.py:

video_source = 0  # 0 for default webcam
📋 Log Player Positions
If logging is enabled, the output will be saved to:

player_tracking_log.csv
