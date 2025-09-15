# Age & Emotion Detection for Movie Theatre

This project detects **age and emotion** of people entering a movie theatre in real time.  
If a person is **under 13** or **over 60**, the system shows a **red box with "Not allowed"**.  
If the age is **13–60**, it also predicts the **emotion** and shows a **green box with emotion label**.  

All results are logged into `theatre_log.csv`.

---

## Features
- Real-time webcam detection using OpenCV
- Age detection using your trained model
- Emotion detection using your trained model
- Tkinter GUI with **Start** and **Stop** buttons
- Automatic logging to CSV (Age, Emotion, Entry Time)

---

## Project Structure

age-emotion-theatre/
│
├── models/
│   ├── age_model.h5
│   ├── emotion_model.h5
│
├── theatre_detection.py       # main Tkinter app
├── requirements.txt           # dependencies
├── theatre_log.csv            # will be created automatically
├── README.md                  # documentation


---

## ⚙️ Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/das-webber/Age-and-Emotion-Detection-for-Movie-Theatre.git
   cd Age-and-Emotion-Detection-for-Movie-Theatre

2. Install dependencies:
   pip install -r requirements.txt

3.Place pre-trained models inside the models/ folder:

    ->models/emotion_model.h5

 Usage

Run the notebook:

    Age_And_Emotion_Detection_for_movie_Theatre
    
    Click Start Detection → Live camera feed starts.
    Click Stop Detection → Detection stops, data saved to CSV.

 Output:

Under 13 / Over 60 → Red box + "Not allowed"

Age 13–60 → Green box + Emotion label

Log saved as theatre_log.csv with:
      
      Age, Emotion, EntryTime

