# Face_Recognize
- [**About Project**](#about-project)
  - [**About Model**](#about-model)
  - [**About My Technique**](#about-my-technique)
- [**Result**](#result)
- [**Reference**](#reference)
# About Project
- Face Recognize is one of the famous application of Computer Vission in AI, It help us detect the person that we want to know.
- We can not use normal Classify (image is labeled with name and train to get the name) because it hardly to add new face (we should train the model again and again when we add new person). More and more, it take a lot of parameter for final output (Example, we have 1000000 employees at a company, so we have 1000000 name to classify).
- So I use ARC Face model have train with a lot of face (including ASIA face) to get the embedding vector (just get feature of face) and compare with all embedding vector in database. As the result, we needn't train model again and again when we add a new person, we just add image of his / her face and get his / her embedding vector.
![alt text](https://github.com/duytran1332002/Face_Recognize/blob/main/image1.PNG?raw=true)
- I use Yolov3 to detect the position of face to:
![alt text](https://github.com/duytran1332002/Face_Recognize/blob/main/image2.PNG?raw=true)
## About Model
- Model embedding: **ARC FACE** model.
- Model detection: **YOLOV3.**
- Compare function: **consine similarity, Mean Square Error**.
## About My Technique:
- Tensorflow: v12.8
- Python: 3.8
- cuda: 11.2
# Result
![alt text](https://github.com/duytran1332002/Face_Recognize/blob/main/result.png?raw=true)
# Reference
- AI Viet Nam: https://www.facebook.com/aivietnam.edu.vn
- Arc Face Model: https://sefiks.com/2020/12/14/deep-face-recognition-with-arcface-in-keras-and-python/
- Model Yolov3 Face Detection: https://github.com/chinmaykumar06/face-detection-yolov3-keras
