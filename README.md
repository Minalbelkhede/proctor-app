# proctor-app

This is a comprehensive proctoring system built using Python. It integrates several functionalities, including:

1. **Webcam Monitoring**: It uses OpenCV to capture video from the user's webcam and perform face detection. If no face is detected, it issues warnings and can terminate the exam.

2. **Screen Recording**: The system captures the user's screen activity using PyAutoGUI and OpenCV, storing it in a video file while ensuring the file is non-deletable.

3. **Audio Monitoring**: It monitors the microphone for sound activity using PyAudio, issuing warnings if sound is detected during the exam.

4. **Keyboard Monitoring**: The system checks for the presence of specific key presses that may indicate unauthorized activity.

5. **Logging**: It logs all activities and warnings to a text area and saves them to an HTML file upon exam completion.

6. **User Interface**: The proctoring system has a Tkinter GUI for providing instructions, entering the exam URL, and displaying log messages.

7. **Exam Start and End Management**: The system allows the user to start the exam by entering a valid exam URL and manages the exam lifecycle, including warnings and termination conditions.

### Key Features:
- **Face Detection**: Utilizes Haar cascades to detect faces in real-time.
- **Hotkey Support**: The user can exit the exam with the 'Esc' key.
- **Instructions Display**: Provides detailed instructions for taking the exam.
- **Multithreading**: Uses threads for monitoring webcam, sound, and keyboard input concurrently.

### Usage:
To run this proctoring system, ensure you have the necessary libraries installed (such as `opencv-python`, `numpy`, `pyaudio`, `pyautogui`, `keyboard`, and `Pillow`).


The provided code implements a **proctoring system** that can be used for online examinations. Its primary purpose is to ensure the integrity of the exam-taking process by monitoring the candidate's behavior and environment during the test. Here's a breakdown of how this code can be used:

### Use Cases

1. **Online Examinations**:
   - Schools, universities, or organizations can use this system for conducting online exams where monitoring is essential to prevent cheating.

2. **Remote Assessments**:
   - It can be employed in scenarios where assessments are conducted remotely, ensuring that candidates adhere to exam protocols.

3. **Proctoring Services**:
   - Companies offering proctoring services can utilize this code as part of their platform to monitor test-takers effectively.

### Key Features for Usage

1. **Webcam Monitoring**:
   - The system captures video from the candidate's webcam to ensure that they are present and to detect any unauthorized individuals or activities during the exam.

2. **Screen Recording**:
   - It records the candidate's screen activity, allowing for review if there are any suspicions of cheating or misconduct.

3. **Sound Monitoring**:
   - The microphone is monitored to detect any sounds that might indicate unauthorized assistance or distractions.

4. **Keyboard Monitoring**:
   - The system can detect specific key presses that may signal attempts to cheat or access unauthorized resources.

5. **Warning System**:
   - The system issues warnings based on different triggers (e.g., no face detected, sounds, unauthorized key presses) and can terminate the exam if the warning threshold is exceeded.

6. **Logging**:
   - All activities, warnings, and logs are stored for later review, providing a clear record of the exam session.

7. **User Interface**:
   - The Tkinter GUI provides a user-friendly interface for candidates to start their exams, view instructions, and see log messages in real-time.

### Steps to Use the Code

1. **Setup**:
   - Ensure you have Python installed along with the required libraries: `opencv-python`, `numpy`, `pyaudio`, `pyautogui`, `keyboard`, and `Pillow`.

2. **Run the Code**:
   - Execute the script in a Python environment. This will open a window displaying exam instructions and prompting for the exam URL.

3. **Enter Exam URL**:
   - Input the URL of the exam to be taken. The system will open this URL in a web browser.

4. **Start the Exam**:
   - Click the "Start Exam" button after ensuring the webcam is operational. The monitoring process will begin.

5. **Take the Exam**:
   - Complete the exam while the system monitors for any violations. Follow the instructions provided.

6. **End the Exam**:
   - The exam can be submitted by pressing the 'Esc' key, which will trigger the system to save logs and stop monitoring.

### Considerations

- **Privacy and Compliance**: Before using this system, it's important to consider privacy laws and regulations regarding video and audio recording, especially in educational and professional settings.
- **Technical Requirements**: Ensure that candidates have the necessary hardware (webcam, microphone) and software installed to run the proctoring system effectively.
- **User Training**: Candidates may need training or guidance on how to use the system and understand the monitoring processes involved.

Overall, this proctoring system serves as a robust solution for maintaining integrity during online assessments. 

Thank you for Reading... Happy learning!
