# 🧠 AI-Powered Second Brain Project

This project is designed to help users manage and interact with their knowledge effectively, particularly through highlights from research papers, books, or any other documents. Users can generate research summaries, essays, and detailed insights based on specific topics. The project was demoed during a hackathon and you can find a video of the demo [here](https://youtube.com/your-demo-link).

---

## 📑 Table of Contents
1. [General Info](#general-info)
2. [Screenshots](#screenshots)
3. [Demo](#demo)
4. [Technologies and Tools](#technologies-and-tools)
5. [Setup](#setup)
6. [Process](#process)
7. [Code Examples](#code-examples)
8. [Features](#features)
9. [Status](#status)
10. [Contact](#contact)

---

## 📜 General Info
This project builds an interactive tool that allows users to create research summaries, essays, and relevant highlights using AI. By inputting a topic or section, users can retrieve structured information from a collection of highlights. It supports different essay formats, summary generation, and more, utilizing LlamaIndex for efficient querying and embedding techniques.

Key features include:
- Topic-based research highlights
- Detailed summary generation
- Essay creation with user-defined word limits and formats

The project was demoed during the TEDAI For Good Hackathon, focusing on leveraging AI for knowledge management.

---

## 📸 Screenshots
Here are some visuals from the project.

1. **Dashboard Interface**  
   ![Dashboard](https://via.placeholder.com/600x300)
   
2. **Research Highlights Tab**  
   ![Research Highlights](https://via.placeholder.com/600x300)
   
3. **Essay Generation Tab**  
   ![Essay Generator](https://via.placeholder.com/600x300)

---

## 🎥 Demo
You can view a full demo of the project [on YouTube](https://youtube.com/your-demo-link).

---

## 🛠 Technologies and Tools
The project leverages the following technologies and tools:

- **Python**: Core language for backend processing
- **Streamlit**: Web framework for building interactive UI
- **LlamaIndex (GPT Index)**: Used for querying and interacting with documents
- **Transformers**: Used for embedding text and similarity matching
- **Google Docs API**: To pull document highlights directly
- **Pandas**: Data processing and management
- **Spacy**: For Named Entity Recognition (NER)
- **Hugging Face Transformers**: For text embeddings and further AI-driven features

---

## ⚙️ Setup
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/second-brain-ai.git




---

## 📊 Process

### 1. **Data Collection**:
   The highlights are sourced from Google Docs using the Google Docs API, allowing easy import of reading highlights, or uploaded manually into the system.

### 2. **Data Preprocessing**:
   The raw text highlights undergo preprocessing using:
   - SpaCy for text cleaning and Named Entity Recognition (NER).
   - Custom functions to clean and standardize the text.

### 3. **Querying with LlamaIndex**:
   The LlamaIndex Query Engine is used to efficiently search through the document highlights. 
   It helps retrieve the most relevant information using text-based searches for research papers, summaries, or essays.

### 4. **Generating Summaries and Essays**:
   Based on the user's input, the system generates:
   - Summaries of specific topics within the text.
   - Custom essays using the processed highlights, following the user's preferences in style and length.

### 5. **User Feedback Integration**:
   After generating responses (highlights, summaries, essays), users can provide feedback. This feedback loop helps refine future responses.

---

## 🖥️ Code Examples

### Extracting Named Entities:
```python
import spacy

nlp = spacy.load("en_core_web_sm")

def extract_entities(text):
    doc = nlp(text)
    return [(ent.text, ent.label_) for ent in doc.ents]

df_highlights['entities'] = df_highlights['text'].apply(extract_entities)


---

## ✨ Features

- Pull and preprocess Google Docs highlights.
- Efficient searching and summarizing of text using LlamaIndex.
- Generate research papers and essays based on user inputs.
- User feedback integration for refining results.
- Multiple essay types (research, editorial, etc.) with configurable word limits.
- Customizable output formats (bullet points, plain text, etc.).

---

## 🚧 Status

This project is currently in development. New features like direct export to Word and integration with other knowledge management tools are planned.

---

## 📧 Contact

Created by [Harsh Gupta](https://www.linkedin.com/in/harshgupta). Feel free to contact me for any questions or collaboration opportunities.

   
