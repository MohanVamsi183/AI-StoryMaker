# AI StoryMaker

**Generating coherent stories from image sequences using vision–language models**

AI StoryMaker is an end-to-end application that converts a sequence of images into a short, coherent story. The system combines image captioning and large language models to understand visual scenes and generate narrative text conditioned on user-selected moods.

**Live Demo (Hugging Face Space):**
[Try the AI StoryMaker on Hugging Face Spaces](https://mohanvamsivp-ai-storymaker.hf.space)

---

## Overview

The project takes multiple images as input, automatically extracts semantic descriptions for each image, and generates a complete short story that connects all scenes in a consistent narrative. Users can control the tone and style of the story through predefined mood settings.

---

## Key Features

* Upload multiple images (5–10 recommended)
* Automatic scene understanding using vision–language models
* Short story generation (200–250 words)
* Mood-based narrative control:

  * Romance
  * Comedy
  * Scary
  * Action
  * Cartoonish
* Interactive web interface built with Gradio
* Deployed on Hugging Face Spaces

---

## System Architecture

1. **Image Input**
   Users upload a sequence of images through the web interface.

2. **Image Captioning**
   Each image is processed using BLIP to generate a descriptive caption.

3. **Prompt Construction**
   Captions are combined with a mood-specific prompt template.

4. **Story Generation**
   The structured prompt is passed to Gemma-2B-IT to generate a coherent narrative.

5. **Output Display**
   The generated story and corresponding scene captions are displayed to the user.

---

## Technology Stack

### Models

* BLIP (Salesforce) – Image Captioning
* Gemma-2B-IT (Google) – Story Generation

### Frameworks and Tools

* Python
* PyTorch
* Hugging Face Transformers
* Gradio
* Hugging Face Spaces
* BitsAndBytes (for quantized inference)


---

## Deployment

The application is deployed on Hugging Face Spaces.

* Access tokens are stored securely using Space Secrets
* Automatically runs on CPU or GPU depending on availability
* Uses quantization when GPU is available to reduce memory usage


---

## Performance Notes

* Initial inference may be slower due to model cold start
* CPU-based Spaces are slower than GPU-based Colab environments
* Performance improves after models are loaded into memory


---

## License

This project is licensed under the MIT License.

---

## Author

**Mohan Vamsi Varadaraju Priya** /
MS in Applied Machine Learning /
University of Maryland, College Park /

GitHub: [Check out my Github account](https://github.com/MohanVamsi183)
Hugging Face: [Check out my Hugging Face account](https://huggingface.co/mohanvamsivp)
