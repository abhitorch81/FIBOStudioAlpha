FIBO Studio Alpha

JSON-Native Visual Control Platform built on Bria FIBO

FIBO Studio Alpha is a production-oriented visual generation platform that uses structured JSON prompts and LLM translation to deliver deterministic, controllable, and reproducible image generation workflows.
It demonstrates how Bria FIBO can be used to build automated, scalable, professional visual pipelines for developers and artists.

🚀 Key Idea

JSON is the single source of truth.
Natural language and images are translated into structured JSON via an LLM, and that JSON drives the entire visual generation pipeline.

✨ Features

JSON-Native Image Generation
All images are generated from structured JSON prompts, not free-text.

LLM-Powered Translation

Natural language → JSON

Image → JSON

JSON-preserving refinement

Camera-Level Controllability
Explicit control over camera angle, lens, lighting, color palette, and composition.

Deterministic & Reproducible
Seeded execution ensures the same JSON always produces the same result.

Professional Workflows

Generate

Refine

Inspire (image-to-image via JSON)

Artist Workflow Integration
JSON prompts can be exported into a ComfyUI-style node graph for post-processing and creative iteration.

🧠 Why FIBO Studio?

Most AI image tools rely on unstructured prompts, making them unpredictable and unsuitable for production.
FIBO Studio shows how structured prompts + LLM translation transform image generation into a controllable, scalable, professional pipeline.
🔄 Core Workflows
1. Generate

Natural language → structured JSON → image

2. Refine

Existing JSON + refinement instruction → updated JSON → image
(Only modified fields change; no prompt drift.)

3. Inspire

Image → structured JSON → controlled variations

🛠️ Tech Stack
Languages

Python

Frameworks & Libraries

PyTorch

Hugging Face Diffusers

Hugging Face Transformers

Accelerate

Pillow

Gradio

Hugging Face Hub

Models

Bria FIBO (briaai/FIBO)

Bria FIBO VLM Prompt-to-JSON (briaai/FIBO-VLM-prompt-to-JSON)

Platforms

Google Colab (GPU)

Hugging Face (model hosting & access)

▶️ Running the Project (Colab)

Open Google Colab with GPU enabled

Authenticate with Hugging Face:
{
  "subject": "running shoe",
  "style_medium": "photograph",
  "camera_angle": "low",
  "lens_focal_length": "85mm",
  "lighting": {
    "key_light": "soft rim light"
  },
  "color_palette": ["black", "cyan accents"],
  "composition": {
    "rule_of_thirds": true
  }
}
🏆 Hackathon Alignment

FIBO Studio Alpha directly targets:

Best JSON-Native or Agentic Workflow

Best Controllability

Best New User Experience / Professional Tool

Best Overall (stretch)

🔮 What’s Next

Expanded JSON schema & validation

Agent-assisted creative workflows

Deeper ComfyUI integration

Batch & campaign-scale generation

Collaboration, versioning, and auditability
