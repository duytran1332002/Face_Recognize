# Face_Recognize
- [**About Project**](#about-project)
  - [**About Model**](#about-model)
  - [**About My Technique**](#about-my-technique)
- [**Result**](#result)
- [**Reference**](#reference)
# About Project
- Face Recognize is one of the famous applications of Computer Vision in AI, It helps us detect the person that we want to know.
- We can not use normal Classify (the image is labeled with a name and trained to get the name) because it is harder to add a new face (we should train the model again and again when we add a new person). More and more, it takes a lot of parameters for the final output (for example, we have 1000000 employees at a company, so we have 1000000 names to classify).
- So I used the ARC Face model have trained with a lot of faces (including ASIA faces) to get the embedding vector (just get the feature of the face) and compare it with all embedding vectors in the database. As the result, we needn't train the model again and again when we add a new person, we just add an image of his / her face and get his / her embedding vector.
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
