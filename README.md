# Embedded Intelligent Microscopy System for Identification and Counting of Microscopic Marine Organisms

An **AI-powered intelligent microscopy system** for **real-time plankton monitoring**.  
Automatic species identification of microscopic marine organisms . This project leverages **YOLOv8, Raspberry Pi, and OpenCV** to detect, classify, and monitor plankton species in microscopy images and live streams.

---

##  Features
-  **Multi-class Plankton Detection** using YOLOv8  
-  **Real-time monitoring** from microscopy feeds  
-  **UI Integration Ready** for smooth deployment in external apps  
-  **Portable Deployment** on Raspberry Pi and edge devices  
-  **Clean & Modular Codebase** (notebooks + scripts + inference)  
-  **Dataset Handling** for custom plankton datasets  

---


## ⚙️ Setup & Installation

1. **Clone the repository**
 ```bash
   git clone https://github.com/<your-username>/plankton-vision.git
   cd plankton-vision
```
2.*Create a virtual environment & install dependencies*
   ```bash
   python -m venv venv
   source venv/bin/activate    # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
 ```
3.*Download trained weights*
   ```bash
   scripts/download_weights.sh
```
4.*Running Inference*

Using the Notebook

Open notebooks/model_clean.ipynb.

Run cells in order.

The demo saves results into results/demo_result.jpg.
  ```bash
python src/inference.py --weights weights/best.pt --source assets/example.jpg
```
5.*Training the Model*

Place your dataset in data/ (YOLOv8 format).

Open notebooks/model_clean.ipynb.

Run training cells.

Trained weights will be saved under weights/.

6.*Tech Stack*

Deep Learning → PyTorch, YOLOv8 (Ultralytics)

Computer Vision → OpenCV, Pillow

Visualization → Matplotlib, Seaborn

Deployment → Raspberry Pi, Python


