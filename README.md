# aura-model-
we have an team project for hackarthon we create a web for aura model using ml 
AURA PHOTO RATING (onine app)

1. Put rating_model_single.onnx (from Colab: Aura project/runs/fold1) in the "model" folder.
   If you leave it in Downloads or in your project folder, the launcher will try to find it.
2. Mac: double-click "Start Aura (Mac).command". The browser opens by itself.
   If macOS blocks it: right-click the file, choose Open, then Open again.
   Still blocked? Open Terminal, type: bash   (then a space), drag the .command file into the window, press Enter.
   Windows: double-click "Start Aura (Windows).bat" (needs Python 3).
3. Wait for "Ready." then choose a frontal face photo.
Do not open index.html directly. It only works through the launcher.

The first start downloads a small face detector, so it needs internet once.
The number is an estimate of the average 1-5 rating raters in SCUT-FBP5500 gave to frontal face photos.
It is not a measure of a person. Photos stay on this computer.
The model is trained on research-licensed data; check the SCUT-FBP5500 license before commercial use.
Bundled: ONNX Runtime Web 1.19.2 (MIT), MediaPipe Tasks Vision 0.10.3 (Apache-2.0).
