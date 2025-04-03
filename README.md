Hand Gesture Recognition using OpenCV, MediaPipe & TensorFlow

This project is a real-time Hand Gesture Recognition system that uses OpenCV, MediaPipe, and TensorFlow to detect and classify hand gestures from a webcam feed. The model can recognize different hand gestures and can be used for applications like virtual controls, sign language recognition, and human-computer interaction.

Features:
 Real-time hand tracking using MediaPipe Hands
 Deep learning-based gesture classification using a CNN model
 Fast and efficient processing with OpenCV

Technologies Used

 OpenCV – For capturing and processing video frames

 MediaPipe – For detecting hand landmarks

 TensorFlow/Keras – For training and loading the gesture classification model

 NumPy – For numerical operations

 How It Works

Capturing Video Input

OpenCV initializes the webcam and continuously captures frames.

The frames are flipped horizontally to create a mirror effect.

Hand Detection and Landmark Extraction

MediaPipe Hands detects the presence of a hand in the frame.

If a hand is detected, the model extracts 21 landmark points representing key positions on the hand.

Data Preprocessing

The extracted landmark coordinates are normalized based on the frame dimensions.

The processed landmark data is formatted to match the input format expected by the trained CNN model.

Gesture Prediction

The pre-trained CNN model predicts the gesture class based on landmark positions.

The highest probability class is selected and mapped to a gesture name.

Displaying Results

The predicted gesture name is displayed on the screen.

Hand landmarks and connections are drawn on the video frame for visualization.

User Interaction

The program continues to process video frames until the user presses 'q' to exit.
