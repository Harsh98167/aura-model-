AURA – AI-Powered Photo Rating System

This is an ML-powered application that estimates the average human rating of a frontal-face photograph using a trained machine learning model.

## Setup Instructions

1. Download or obtain the `rating_model_single.onnx` file from `Aura project/runs/fold1` in Google Colab.
2. Place the model file inside the project's `model` folder.
3. If you cannot find the model file, the launcher will also attempt to locate it in your Downloads folder or main project directory.

## How to Run the Application

**For macOS:**
1. Double-click `Start Aura (Mac).command`.
2. Your default browser will open automatically.
3. If macOS blocks the application, right-click the file, select **Open**, and confirm by selecting **Open** again.
4. Alternatively, open Terminal, type `bash` followed by a space, drag the `.command` file into Terminal, and press Enter.

**For Windows:**
1. Double-click `Start Aura (Windows).bat`.
2. Make sure Python 3 is installed on your computer.
3. Wait until the application displays **Ready**.

## How to Use AURA

1. Wait for the application to display **Ready**.
2. Upload a clear, frontal-face photograph.
3. The face detector checks the uploaded image.
4. The ONNX model processes the photograph and generates an estimated rating between **1 and 5**.

## Important Information

- Do not open `index.html` directly. Always launch the application using the appropriate launcher.
- An internet connection is required during the first launch to download the face detector.
- The rating represents an estimate of the average ratings given by human raters in the SCUT-FBP5500 dataset.
- The score evaluates the photograph according to patterns learned from the dataset. It does not measure a person's identity, personality, worth, or overall attractiveness.
- Uploaded photographs remain on the local computer and are not sent to an external server by the application.

## Technologies and Licenses

- **ONNX Runtime Web 1.19.2** – MIT License
- **MediaPipe Tasks Vision 0.10.3** – Apache License 2.0
- **Machine Learning Model:** `rating_model_single.onnx`
- **Training Dataset:** SCUT-FBP5500

**License Notice:** The model is trained using research-licensed data. Review the SCUT-FBP5500 dataset license and applicable model-use restrictions before using AURA commercially.
