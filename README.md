# 📘 AI-Powered PDF Image Explanation Video Generator

This project automatically converts **PDF images** into a **professional narrated video** using **AI explanations** and **text-to-speech narration**.

---

## 🚀 Features

- 📄 Extracts all images from a given PDF using **PyMuPDF**  
- 🤖 Generates intelligent explanations for each image using **Google Gemini AI**  
- 🎙️ Converts explanations into professional voice narration using **Edge TTS**  
- 🎬 Combines images, explanations, and audio into a high-quality **MP4 video** using **MoviePy**  
- 🖼️ Adds title, figure numbers, and end slide for a clean professional finish  

---

## 🧩 Workflow

1. **Cell 2** → Extracts images from PDF  
2. **Cell 3** → Generates AI explanations (Gemini API)  
3. **Cell 4–5** → Skips text extraction (image-based narration only)  
4. **Cell 6** → Converts text to speech using **Edge TTS**  
5. **Cell 8** → Merges images, audio, and text into a **final HD video**

---

## 💡 Example Use Case

Upload a research or technical PDF with diagrams →  
The system explains each image and produces a **video presentation** automatically.

---

## ⚙️ Technologies Used

- **Python 3**
- **PyMuPDF (fitz)** – PDF image extraction  
- **Google Gemini API** – AI explanation generation  
- **Edge TTS** – Text-to-speech narration  
- **MoviePy & PIL** – Video creation and image rendering  





## 📦 Output

🎥 `professional_image_explanation_video.mp4`  
A full HD video with synchronized narration, figure explanations, and polished visuals.


