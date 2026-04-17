Video Object Removal 🎥

This project allows users to remove unwanted objects from videos by simply drawing a bounding box around the object. The system automatically tracks and removes the object across frames using deep learning techniques.

✨ Features
Remove objects from videos easily
Works on both image sequences and video files
Uses object tracking + video inpainting
Simple command-line interface
🛠️ Tech Stack
Python
PyTorch
Computer Vision
Deep Learning (Object Tracking + Inpainting)
📂 Project Setup
1. Clone the repository
git clone https://github.com/Anjalisharma3463/video-object-removal.git
cd video-object-removal
2. Install dependencies

Go inside folders and run setup scripts:

cd get_mask
bash make.sh

cd ../inpainting
bash install.sh

cd ..
📥 Download Pretrained Models

Download required models:

SiamMask model
Inpainting model

👉 Place them inside a folder named:

cp/
▶️ How to Run
Run on dataset:
python demo.py --data data/Human6
Run on video:
python demo.py --data data/bag.avi
⚙️ Optional Parameter
--mask-dilation

Example:

python demo.py --data data/Human6 --mask-dilation 24

👉 This helps improve object removal edges.

🧠 How It Works (Simple Explanation)
User selects object using bounding box
Model tracks object across frames
Mask is generated
Inpainting fills removed area
Final clean video is generated
📸 Results
Object tracking
Object removal
Smooth background reconstruction
🙏 Credits

This project is based on:

SiamMask
Deep Video Inpainting
👩‍💻 Author

Anjali Sharma

GitHub: https://github.com/Anjalisharma3463
LinkedIn: https://www.linkedin.com/in/anjali-sharma-760a06238