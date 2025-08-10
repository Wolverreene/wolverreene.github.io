---
layout: page
title: Chatbot using RAG
description: Designed and implemented a chatbot tailored to the specific needs of my Department (SINES) in University (NUST). Collected data using Google Forms, online scrapping, and self-collection. Used Retrieval Augmented Generation to enhance Chat Bot design. Utilized OpenAI�s GPT 3.5-Turbo as Large Language Model.
img: assets/img/meri/chatbot.png
importance: 1
category: work
---

## Features

- **Custom Knowledge Base** from:
  - Official SINES website (web crawling)
  - Manually collected data via **Google Forms** (lab functions, ongoing research, equipment)
  - Physical **mapping of department building** (labs, offices, restrooms, extinguishers, etc.)
- **RAG-based Retrieval Pipeline** to fetch accurate context from documents
- **GPT-3.5 Turbo Integration** via API for natural language responses
- **Interactive UI** built using [Panel](https://panel.holoviz.org/) for smooth user experience
- **Multiple RAG Chain Modes**: `stuff`, `map_reduce`, `refine`, `map_rerank`

- ## How to Run

### Prerequisites

- Python 3.8+
- OpenAI account with access to API key
- Internet connection
- Install the required library:

```bash
!pip install langchain
```

### Steps to Run

1. Open the Notebook: 'ChatbotNLP.ipynb'
2. Set your OpenAI API Key:

   Replace the placeholder in the notebook with your API key:

```bash
params[variable] = params.get(variable, os.environ.get(variable, "placeholder"))
```

3. Run the Web App:
4. Open Anaconda Prompt or Python terminal and run:

```bash
panel serve chatbotNLP.ipynb
```

5. Access the Chatbot:
   Copy the URL shown in the terminal (e.g., http://localhost:5006/ChatbotNLP) and open it in a browser.

Tested on Windows OS. Compatibility with other operating systems may require adjustments.

## Results

Screenshots of interface:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/meri/chatbot1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    General Query
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/meri/chatbot.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
     Contact Info
</div>

## Technology Used

- OpenAI GPT-3.5 Turbo
- LangChain
- Panel (for UI)
- PDF Text Extraction & Chunking
- Manual and Automated Data Collection

## Use Cases

- Students exploring research labs or projects
- Faculty contact and departmental directory lookup
- Visitors navigating the department building
- Admins quickly answering common questions

## Notes

- The OpenAI API key used during development has been excluded for security.
- You must insert your own API key as described above.
- The project was tested and confirmed to work on Windows OS.

{% endraw %}
