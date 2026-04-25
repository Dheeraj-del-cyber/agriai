🌿 Smart Agriculture Assistant

An offline-first AI-powered system for crop disease detection, intelligent advisory, and crop recommendation — designed to assist farmers even without internet access.

---

🧩 Problem

Farmers often struggle to get timely expert advice, which leads to:

- Incorrect disease identification
- Overuse of pesticides
- Reduced crop yield

This problem becomes critical in rural areas with poor or no internet connectivity.

---

💡 Solution

We developed a smart agriculture assistant that:

- Detects plant diseases using CNN models
- Validates input images using image processing techniques
- Provides AI-based advisory (LLM / Knowledge Base)
- Recommends suitable crops using Machine Learning
- Works offline-first, with optional online enhancements

---

🧠 System Architecture

"Pipeline" (assets/pipeline.png)

---

⚙️ Tech Stack

- 🧠 AI/ML: TensorFlow Lite, Scikit-learn
- 🖼️ Image Processing: OpenCV (Laplacian Variance, Green Pixel Ratio, TTA)
- 🤖 LLM: Groq API (Online) + Local Knowledge Base (Offline)
- 🌾 ML Model: Random Forest (Crop Recommendation)
- 🗄️ Storage: JSON / SQLite
- 🌐 Frontend: HTML, CSS, JavaScript
- 🔙 Backend: Python

---

🔬 Key Features

- ✅ Offline-first architecture
- ✅ Image validation (blur detection + leaf detection)
- ✅ Disease detection using CNN
- ✅ AI-powered advisory system
- ✅ Crop recommendation using ML
- ✅ Multi-language support
- ✅ Chatbot (Online + Offline fallback)
- ✅ Fast and lightweight performance

---

🔄 How It Works

1. User uploads a leaf image
2. Image is validated:
   - Blur detection (Laplacian Variance)
   - Leaf detection (Green Pixel Ratio)
3. Valid image is processed using CNN
4. Disease + confidence score is generated
5. Advisory is generated using:
   - Groq API (if online)
   - Local Knowledge Base (if offline)
6. Crop recommendation:
   - Online → Data fetched via APIs
   - Offline → Manual input from user
   - Processed using Random Forest model
7. Final results are displayed in the selected language

--

🛠️ Setup

git clone https://github.com/dheeraj-del-cyber/agriai.git

cd https://github.com/dheeraj-del-cyber/agriai.git

pip install -r requirements.txt
python app.py

---
🚀 Future Scope

- Fully offline LLM integration
- IoT-based smart farming integration
- Improved model accuracy with larger datasets

---


