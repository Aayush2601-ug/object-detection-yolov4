# 🚗 Real-Time Object Detection using YOLOv4 + OpenCV

A real-time **object detection system** built using **YOLOv4** and **OpenCV**, capable of detecting multiple object classes (cars, people, traffic signs, etc.) with high accuracy.  
This project includes full inference code, visualization tools, pre-trained YOLOv4 configuration files, and a set of test images for immediate experimentation.

---

## 📌 Features
- ⚡ **Real-time object detection** with YOLOv4  
- 🎯 **Multi-class detection** using COCO dataset labels  
- 🖼 Draws bounding boxes + confidence scores  
- 🧪 Includes test images in the `test/` folder  
- 📓 Complete Jupyter Notebook for experiments (`Object_detection_final.ipynb`)  
- 🔧 Fully customizable (confidence threshold, NMS, model config)  
- 🚀 Works on CPU  

---

## 🧠 Model Details

This project uses:
- **YOLOv4 architecture**
- Pre-trained weights trained on **COCO dataset (80 classes)**
- OpenCV's DNN module for fast inference

Key files:
- `yolov4.cfg` — YOLOv4 model architecture  
- `coco.names` — Class labels  
- **Weights file** (downloaded externally, see instructions below)  
- `Object_detection_final.ipynb` — Main notebook with detection pipeline  
- `data.csv` — Detection logs (optional)  

YOLOv4 is optimized for speed + accuracy, making it ideal for real-time applications like:
- Autonomous driving  
- CCTV analytics  
- Traffic monitoring  
- Object tracking systems  

---

## 📂 Project Structure
```

├── test/                            # Test images for object detection
├── yolov4.cfg                       # YOLOv4 configuration file
├── coco.names                       # COCO dataset class labels
├── Object_detection_final.ipynb     # Main object detection notebook
├── data.csv                         # Optional detection logs
└── README.md

````

---

## 🛠 Installation

### 1️⃣ Clone this repository
```bash
git clone https://github.com/<your-username>/object-detection-yolov4.git
cd object-detection-yolov4
````

### 2️⃣ Install dependencies

```bash
pip install opencv-python numpy matplotlib
```

(Optional accelerated version)

```bash
pip install opencv-contrib-python
```

### 3️⃣ Download YOLOv4 weights

Download from official Darknet repository:

👉 [https://github.com/AlexeyAB/darknet/releases/](https://github.com/AlexeyAB/darknet/releases/)

File needed:

```
yolov4.weights
```

Place it inside the project folder.

---

## 🚀 Usage

### Run the notebook

Open:

```
Object_detection_final.ipynb
```

And run all cells to:

✔ Load YOLOv4
✔ Run detection on images
✔ Display results
✔ Modify confidence threshold
✔ Test on custom images from `test/` folder

---

## 🖼 Example Output

Add this image to your repo and reference it here:

```
![Detection Example](test/sample_output.jpg)
```

Or the one you sent:

![Example Detection](1.jpg)

---

## 📊 Dataset & Classes

This model uses **COCO dataset labels**, which include:

* Person
* Car
* Bus
* Truck
* Dog
* Bicycle
* Traffic light
* …and 70+ more classes

See `coco.names` for the full list.

---

## 🔍 How It Works

1. Load YOLOv4 configuration + weights
2. Preprocess input image
3. Perform forward pass through DNN
4. Use NMS (Non-Max Suppression)
5. Draw bounding boxes with class & confidence

This ensures fast + accurate predictions even on CPU.

---

## 🔮 Future Improvements

* Add YOLOv8 or YOLO-NAS model
* Deploy using Streamlit or FastAPI
* Real-time webcam detection
* Object tracking with DeepSORT
* Convert to TFLite for mobile inference

---

## 🤝 Contributors

Developed by **Aayush**.

---

## ⭐ Support

If you found this project useful, please ⭐ the repository.
