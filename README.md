Invisibility Cloak using Python & OpenCV

Make yourself invisible with just a red cloth! ✨
This project demonstrates how computer vision and image processing can create real-time visual effects. Using Python and OpenCV, we detect a specific color (red cloak) and replace it with the captured background, making the object appear invisible — just like Harry Potter’s cloak.


🚀 Features

Real-time invisibility effect using webcam 🎥

Red-colored cloak disappears seamlessly

Background capture for natural effect

Works on any system with Python + OpenCV

Simple, customizable, and beginner-friendly

⚙️ How It Works

Background Capture – At the start, the program records the background for a few seconds.

Color Detection – The cloak’s red color is detected using HSV (Hue, Saturation, Value) color space.

Masking – A mask is created where red regions are separated from the frame.

Replacement – Those masked red areas are replaced by the background pixels.

Result – It looks as if the cloak is invisible in real-time.

🛠️ Tech Stack

Python 3.x 🐍

OpenCV (for image/video processing)

NumPy (for numerical operations)

📂 Project Structure
invisibility-cloak/
│── cloak.py              # Main script
│── requirements.txt      # Dependencies
│── README.md             # Documentation
│── .gitignore            # Ignore unnecessary files

📦 Installation

Clone this repository

git clone https://github.com/your-username/opencv-invisibility-cloak.git
cd opencv-invisibility-cloak


Install dependencies

pip install -r requirements.txt


Run the script

python cloak.py

🎯 Usage Instructions

Place yourself in front of the camera.

Hold a red-colored cloth in front of you.

Stay still for the first 3 seconds (background will be captured).

Watch the magic — the red cloth disappears! 🧙‍♂️

Press Q to exit the program.

🎨 Customization

Change cloak color: Update the HSV range in cloak.py.

Save output video: Use cv2.VideoWriter to record.

Try with different colored backgrounds for cooler effects.

🧪 Example HSV Ranges

For Red cloak (already in code):

lower_red1 = np.array([0, 120, 70])
upper_red1 = np.array([10, 255, 255])
lower_red2 = np.array([170, 120, 70])
upper_red2 = np.array([180, 255, 255])


For Blue cloak:

lower_blue = np.array([94, 80, 2])
upper_blue = np.array([126, 255, 255])


For Green cloak:

lower_green = np.array([25, 52, 72])
upper_green = np.array([102, 255, 255])

📸 Screenshots

(You can add before/after images here)

💡 Future Enhancements

Add GUI with buttons to start/stop cloak

Allow dynamic color selection (trackbars in OpenCV)

Record & save invisibility effect as a video

Support multiple cloaks of different colors

🔍 Learning Outcomes

Understanding of HSV color space

How to use masks in OpenCV

Real-time video capture & manipulation

Basics of image processing pipelines

🏫 Ideal For

College mini-projects

OpenCV beginners

Fun coding practice

Computer vision demonstrations

👨‍💻 Author

Your Name

🔗 GitHub

📧 your.email@example.com

⭐ Contribute & Support

If you liked this project, give it a ⭐ on GitHub and share it with your friends! Contributions are welcome 🚀
