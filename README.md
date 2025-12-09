# Face Detection & Recognition System

A robust Face Detection and Recognition application built with Java, utilizing the power of **JavaCV** (a Java interface to OpenCV). This system supports real-time face detection, data collection, model training, and face recognition using various algorithms like Haar Cascades, LBPH, Eigenfaces, and Fisherfaces.

##  Features

*   **Real-time Face Detection**: Detects faces in live video streams using Haar Cascade Classifiers.
*   **Dataset Creation**: Capture and save face images from the webcam to build a custom dataset.
*   **Model Training**: Train face recognition models (LBPH, Eigenfaces, Fisherfaces) on your captured dataset.
*   **Real-time Recognition**: Identify and label known faces in real-time with confidence scores.
*   **Swing UI**: User-friendly Graphical User Interface for easy operation.

##  Technologies Used

*   **Java**: Core programming language.
*   **JavaCV**: Java wrapper for OpenCV.
*   **OpenCV**: Computer vision library for image processing.
*   **Maven**: Dependency management and build tool.
*   **Swing**: Java GUI toolkit.

##  Prerequisites

*   **Java Development Kit (JDK)**: Version 8 or higher.
*   **Maven**: For building the project and managing dependencies.
*   **Webcam**: Required for capturing images and real-time recognition.

##  Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/muragesh46/Face-Detection.git
    cd Face-Detection
    ```

2.  **Install dependencies:**
    Navigate to the project directory (where `pom.xml` is located) and run:
    ```bash
    mvn clean install
    ```
    *Note: This will download the necessary OpenCV binaries for your platform.*

##  Usage

1.  **Run the Application:**
    You can run the application using Maven:
    ```bash
    mvn exec:java -Dexec.mainClass="com.faceRecogntion.FaceRecognition.App"
    ```

2.  **Using the Interface:**
    *   **Capture & Train Faces**: Click this to open the camera. Enter a Name and ID for the person. The system will capture 30 samples of the face.
    *   **Train Dataset**: After capturing faces, click this to train the recognition model (LBPH) on the collected images.
    *   **Recognize Faces**: Starts the camera and attempts to recognize faces based on the trained model.

##  Project Structure

*   `src/main/java`: Source code for the application.
    *   `App.java`: Main entry point and GUI.
    *   `Capture.java`: Logic for capturing face data.
    *   `Training.java`: Logic for training the recognition model.
    *   `Recognition.java`: Logic for real-time face recognition.
*   `src/main/resources`: Configuration files and data storage.
    *   `haarcascade_frontalface_alt.xml`: Pre-trained face detection model.
    *   `photos/`: Directory where captured face images are stored.
    *   `namedata.csv`: Stores the mapping between IDs and Names.

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
