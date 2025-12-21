# ✨ Generative AI Studio

Welcome to **Generative AI Studio**, a Streamlit-based web application that allows users to explore the capabilities of modern Generative AI models. This project integrates natural language processing and image generation into a single, interactive interface.

🔗 **Live Demo:** [Check out the App on Hugging Face Spaces] -> (https://huggingface.co/spaces/Concordddd/Generative_AI)

## 🚀 Features

The application offers three distinct modes:

### 1. 💬 Chat Mode
Interact with an AI chatbot powered by Google's **Flan-T5** model.
- **Model:** `google/flan-t5-base`
- **Functionality:** Capable of answering questions and engaging in conversation.
- **Tech:** Uses Hugging Face `transformers` for sequence-to-sequence generation.

### 2. 🎨 Art Mode
Generate unique images from text prompts using Stable Diffusion.
- **Model:** `runwayml/stable-diffusion-v1-5`
- **Functionality:** Converts text descriptions into high-quality images.
- **Tech:** Utilizes the `diffusers` library. *Note: Requires a GPU for optimal performance, though it includes a CPU fallback.*

### 3. 🖼️ Image Filter Mode
Upload and edit your own images with classic image processing techniques.
- **Filters Available:**
  - **Grayscale:** Converts image to black and white.
  - **Blur:** Applies a Gaussian blur with adjustable radius.
  - **Color Shift:** Adjusts Red, Green, and Blue channel intensity independently.
- **Tech:** Powered by `Pillow` (PIL).
