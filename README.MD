# OCR with AI Notebooks

This repository contains a collection of Jupyter notebooks demonstrating different approaches to Optical Character Recognition (OCR) using AI models, prompt engineering techniques, and video processing workflows.

## Requirements

These notebooks use **Ollama** to run vision-language models locally.

The default model used throughout the notebooks is:

```text
qwen2.5vl:7b
```

You are free to replace this with any Ollama vision model that best fits your needs. Simply update the model name in the notebook where the Ollama client is initialized.

## Notebooks

### 1. OCR Few Shots Prompting

Demonstrates OCR using **few-shot prompting**, where the model is provided with example inputs and expected outputs before processing new images. This approach can improve extraction accuracy for documents with consistent formatting.

---

### 2. OCR Ollama Notebook

Introduces OCR using an Ollama-hosted vision-language model. This notebook shows the basic workflow for sending images to the model and extracting text using AI instead of traditional OCR engines.

---

### 3. OCR Video Ollama Prompting

Processes video frames with an Ollama vision model to perform OCR over video content. Useful for extracting text from recordings, screen captures, presentations, and other video sources.

---

### 4. OCR Video Splitting EASTOCR

Demonstrates a video OCR pipeline that first splits a video into individual frames and then performs OCR processing. This workflow is useful for handling videos frame-by-frame before text extraction and analysis.

---

### 5. OCR Zero Shot Analysis Images Prompting

Shows how to perform OCR using **zero-shot prompting**, allowing the model to extract and analyze text from images without providing prior examples. This notebook highlights the capabilities of modern vision-language models using prompt engineering alone.

## Getting Started

1. Install and start Ollama.
2. Pull the desired vision model, for example:

```bash
ollama pull qwen2.5vl:7b
```

3. Install the required Python dependencies used by the notebooks.
4. Open the notebooks in Jupyter Notebook or JupyterLab.
5. If you wish to use a different model, replace the model name in the notebook with your preferred Ollama vision model.

## Notes

* The notebooks are independent and can be run separately.
* Some notebooks focus on still images, while others demonstrate OCR workflows for video.
* The prompting techniques shown can be adapted for a variety of OCR and document understanding tasks.
* Performance and accuracy will vary depending on the selected vision model.
