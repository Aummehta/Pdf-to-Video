

# 🎓 EduVisionAI: PDF-to-Educational Video Generator

**EduVisionAI** is an AI-powered automation pipeline that transforms academic **PDF documents** into **professionally narrated educational videos**.
It extracts figures and diagrams, generates intelligent explanations using multimodal AI (Gemini), converts them to natural speech (Edge TTS), and compiles everything into a full HD video presentation using MoviePy.

---

## 📘 Overview

Academic papers often contain complex diagrams and figures that are difficult to interpret for non-experts or visually impaired learners.
**EduVisionAI** aims to bridge this gap by automatically:

* Extracting visual elements (charts, graphs, diagrams) from PDFs,
* Generating concise, educational explanations using **Google Gemini AI**,
* Narrating those explanations with a **natural human-like voice** using **Microsoft Edge TTS**, and
* Compiling them into a **structured, professional video** for enhanced learning accessibility.

This project demonstrates the integration of **multimodal AI**, **speech synthesis**, and **automated video creation** into a single cohesive system.

---

## 🧠 Key Features

✅ **Automated Image Extraction** – Extracts figures and diagrams from academic PDFs using **PyMuPDF**.
✅ **AI-Powered Explanations** – Uses **Google Gemini 2.5 Flash (Vision Model)** to analyze and explain each image.
✅ **Natural Voice Narration** – Converts explanations into high-quality speech using **Microsoft Edge TTS**.
✅ **Professional Video Generation** – Combines visuals, narration, and captions using **MoviePy** and **PIL**.
✅ **Educational Presentation Style** – Includes title slide, figure numbers, clean formatting, and a thank-you end screen.
✅ **Accessibility Enhancement** – Makes academic visuals understandable for students, educators, and visually impaired learners.

---

## ⚙️ Workflow

The project runs as a **cell-by-cell pipeline** (in Jupyter Notebook):

| Step         | Description                                                                | Key Tool / Model        |
| ------------ | -------------------------------------------------------------------------- | ----------------------- |
| **Cell 2**   | Extracts all images from a given PDF                                       | PyMuPDF (fitz)          |
| **Cell 3**   | Generates AI explanations for each image                                   | Google Gemini 2.5 Flash |
| **Cell 4–5** | Skips text extraction and chunking (focuses only on image-based narration) | —                       |
| **Cell 6**   | Converts AI explanations to audio narration                                | Microsoft Edge TTS      |
| **Cell 8**   | Combines visuals, text, and audio into a professional MP4 video            | MoviePy & PIL           |

---

## 🧩 System Architecture

```
PDF Input
   │
   ▼
Image Extraction (PyMuPDF)
   │
   ▼
AI Explanation Generation (Gemini API)
   │
   ▼
Text & Audio Processing (LangChain + Edge TTS)
   │
   ▼
Video Assembly (MoviePy + PIL)
   │
   ▼
🎥 Final Educational Video Output
```

---

## 🧰 Technologies Used

| Component                | Technology              | Purpose                                       |
| ------------------------ | ----------------------- | --------------------------------------------- |
| **Programming Language** | Python 3.10             | Core implementation                           |
| **PDF Handling**         | PyMuPDF                 | Extracts images from PDF pages                |
| **AI Explanation Model** | Google Gemini 2.5 Flash | Vision-based image understanding              |
| **Text Management**      | LangChain               | Coordinates AI responses and processing       |
| **Audio Narration**      | Microsoft Edge TTS      | Converts text to natural-sounding speech      |
| **Video Generation**     | MoviePy, PIL            | Combines images, text overlays, and narration |
| **Development Platform** | Jupyter Notebook        | Sequential execution and debugging            |

---

## 🎯 Output

* **Final File:** `professional_image_explanation_video.mp4`
* **Resolution:** Full HD (1920x1080)
* **Audio:** High-quality AAC narration
* **Includes:**

  * Title Slide
  * Individual Image Segments with Explanations
  * Synced Voiceover
  * End Slide with Credits

---

## 📚 Example Use Case

* Upload a **research paper** or **technical document** containing diagrams.
* EduVisionAI automatically:

  1. Extracts the figures,
  2. Generates educational explanations,
  3. Narrates the content, and
  4. Produces a professional video presentation.

Perfect for:
🎓 **Students** – for understanding complex papers
👩‍🏫 **Teachers** – for creating learning materials
📖 **Researchers** – for academic video summaries
🧑‍🦯 **Visually Impaired Learners** – for accessible content delivery

---

## 🔮 Future Improvements

* 🌍 Multilingual narration support
* 🧑‍🏫 Integration of AI-based teaching avatars
* 🕹️ Real-time adaptive streaming
* ⚡ GPU-accelerated video rendering
* 🧠 Reinforcement feedback for improved explanation accuracy

---

## 🏁 Conclusion

**EduVisionAI** demonstrates how multimodal AI can transform static academic content into dynamic, engaging educational videos.
By integrating visual understanding, natural narration, and automated video generation, this project paves the way for the next generation of **AI-powered educational accessibility tools**.

---

Would you like me to add a **“Setup & Installation”** section next (commands and steps to run it locally)? It’ll make your GitHub README complete and ready to publish.
