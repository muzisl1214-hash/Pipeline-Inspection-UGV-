**🚀 YOLOv8 NCNN Deployment on Raspberry Pi**

**📌 Overview**

This project implements **real-time object detection** using a **YOLOv8 model deployed on Raspberry Pi 4** with the **NCNN framework** for efficient edge inference.

It is designed for **low-power, high-speed applications** such as:

- Pipeline inspection robots
- Crack detection systems
- Edge AI surveillance

**🎯 Key Features**

✔️ Real-time detection on Raspberry Pi  
✔️ Lightweight **NCNN inference (CPU optimized)**  
✔️ Efficient **letterbox preprocessing (no distortion)**  
✔️ Built-in **Non-Maximum Suppression (NMS)**  
✔️ Live **FPS monitoring**  
✔️ Optimized for edge deployment

**🧠 Model Information**

- **Model:** YOLOv8 (Ultralytics)
- **Format:** Converted to NCNN
- **Input Size:** 320×320 (speed optimized)
- **Inference Engine:** NCNN (Tencent)

**🖼️ Demo / Output**

**📷 Live Detection Output**

**⚙️ System Setup**

📌 _Replace these images with your actual screenshots (recommended for GitHub projects)._

**📁 Project Structure**

.

├── ncnn_detect_2.py

├── model.ncnn.param

├── model.ncnn.bin

├── requirements.txt

├── README.md

└── images/

**⚙️ Installation**

**1️⃣ Clone Repository**

git clone https://github.com/your-username/your-repo-name.git

cd your-repo-name

**2️⃣ Install Dependencies**

pip install -r requirements.txt

**3️⃣ Install Picamera2 (if needed)**

sudo apt install python3-picamera2

**4️⃣ Install NCNN**

Follow official guide:  
👉 https://github.com/Tencent/ncnn

**▶️ Usage**

python3 ncnn_detect_2.py

Press **q** to exit.

**⚡ Performance Optimizations**

- Reduced input size → **320 for faster inference**
- Multi-threading enabled → num_threads = 4
- CPU-only execution (Vulkan disabled)
- Efficient preprocessing using **letterbox resizing**

**🔧 Customization**

You can tweak the following parameters in the script:

| **Parameter** | **Description** |
| --- | --- |
| INPUT_SIZE | Increase to 640 for better accuracy |
| CONF_THRESH | Detection confidence threshold |
| NMS_THRESH | Overlap filtering sensitivity |

**🏗️ System Workflow**

Camera → Frame Capture → Preprocessing → NCNN Inference → NMS → Visualization

**📊 Output**

- Bounding boxes
- Class ID + confidence score
- FPS displayed in real time

**🚀 Future Improvements**

- Add **class labels instead of IDs**
- Enable **GPU/Vulkan acceleration**
- Integrate with **autonomous pipeline robot navigation**
- Deploy with **YOLOv9 / quantized models**

**👨‍💻 Author**

**Final Year Project**  
Crack Detection System using Edge AI & Raspberry Pi

**📜 License**

This project is licensed under the **MIT License**

**⭐ Support**

If you find this project useful, consider giving it a ⭐ on GitHub!