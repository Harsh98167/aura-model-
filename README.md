AURA – AI-Powered Photo Rating System

This is an  AI ML-powered application that estimates the average human rating of a frontal-face photograph using a trained machine learning model.

## Setup Instructions

1. Download or obtain the `rating_model_single.onnx` file from `Aura project/runs/fold1` in Google Colab.
2. Place the model file inside the project's `model` folder.
3. If you cannot find the model file, the launcher will also attempt to locate it in your Downloads folder or main project directory.
4. 
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

## HOW TO RUN 

1. Launch the Studio: Open the web app link in any browser or click Open Camera-Ready Tab at the top for instant HTTPS webcam access.
2. Capture or Upload a Portrait: Click Upload Photo to select an image or switch to 2. Live Camera Scan for guided alignment.
3. Align & Auto-Level: Position your face inside the camera reticle until the alignment lock reaches $\ge 88\%$, or click Auto-Level & Center in the crop studio to straighten head tilt.
4. Select Regional Cohort: Use the top-right dropdown menu to switch the active benchmark between Indian / South Asian, East Asian, or Combined Global Corpus to match your geographical region.
5. Run the AI Pipeline: Click Calculate Aura Results to execute the 7-pass TTA neural analysis, 12-biomarker extraction, and pose stabilization.
6. Compare Regional Peers: Open the Dataset Comparison tab and click the regional cohort pills to recalibrate your percentile ranking and $k$-NN matches against local peers.
7. Import Custom Regional Data: Open Documentation & Corpus Details at the top and click Append CSV / JSON to upload custom regional datasets.
8. Re-Train Ensemble Locally: Click Re-Train Max Ensemble inside the documentation modal to instantly update the AI regression and skin-tone debiasing weights using your newly added data.
9. Simulate Styling Uplift: Navigate to the Styling & Jawline Plan tab to view your matched hairstyle recommendations and toggle posture or lighting fixes in the Score Uplift Simulator.
10. Export & Expand: Download your full calibrated JSON report or export your session dataset anytime; every new scan automatically appends to widen your local corpus.

**License Notice:** The model is trained using research-licensed data. Review the SCUT-FBP5500 dataset license and applicable model-use restrictions before using AURA commercially.
