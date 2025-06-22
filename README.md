# 🤖 Real-Time Face Detection using OpenCV DNN (Deep Neural Network)

This project demonstrates **real-time face detection** using a **deep learning-based DNN model** with **OpenCV**. It uses a pre-trained **ResNet-10 SSD** model trained in the **Caffe framework** to detect human faces in live video streams from a webcam.

---

## 📦 Model Files Used

- `deploy.prototxt` – defines the model architecture.
- `res10_300x300_ssd_iter_140000_fp16.caffemodel` – contains the pre-trained weights.

These files are part of OpenCV's official DNN face detector:
- [Download deploy.prototxt](https://github.com/opencv/opencv/blob/master/samples/dnn/face_detector/deploy.prototxt)
- [Download caffemodel](https://github.com/opencv/opencv_3rdparty/blob/dnn_samples_face_detector_20170830/res10_300x300_ssd_iter_140000_fp16.caffemodel)

---

## ⚙️ How It Works

1. The input frame is converted into a 4D blob using `cv2.dnn.blobFromImage()`.
2. The blob is passed through the DNN model.
3. The model returns a list of detections.
4. Faces with confidence above a threshold (e.g., 0.5) are marked with bounding boxes.

---

## 🧰 Technologies Used

- Python
- OpenCV (`cv2.dnn` module)
- Caffe Model (SSD with ResNet-10 backbone)

---

## 🚀 Getting Started

### 📦 Installation

Install OpenCV via pip:

```bash
pip install opencv-python
