# NLP Project

## Overview

This repository contains a series of Jupyter notebooks focused on various Natural Language Processing (NLP) tasks. The primary areas of exploration include Named Entity Recognition (NER) using BERT, dataset creation for NER, and fine-tuning Large Language Models (LLMs).

## Contents

- **BERT_NER.ipynb**: This notebook demonstrates the implementation of Named Entity Recognition using the BERT model. It covers data preprocessing, model training, and evaluation. The training is performed on a dataset created with an LLM. The model used is **BioBERT**, which is pre-trained on healthcare-related documents. The notebook includes:
  - Data loading and preprocessing
  - Tokenization using BERT
  - Model fine-tuning
  - Evaluation using accuracy metrics

- **Creazione_Dataset_Ner.ipynb**: This notebook focuses on creating a dataset for NER tasks in **IOB format**. The dataset is intended for training BERT/BioBERT models. The steps include:
  - Extracting text from PDFs while ignoring tables
  - Using OpenAI’s GPT for zero-shot entity annotation
  - Defining entity categories: **problema (problem), esame (exam), operazione (operation), farmaci (medications)**
  - Formatting data for model training

- **FinetuningLLM.ipynb**: This notebook provides a guide on **fine-tuning an LLM using distillation**. It leverages **Unsloth AI** to fine-tune a model on responses generated by **Gemini or GPT-4**, using **LoRA (Low-Rank Adaptation)**. The approach includes:
  - Installing necessary libraries
  - Data formatting with chat templates
  - Training with phrase-by-phrase adaptation
  - Future consideration: full-context fine-tuning

## Requirements

To run the notebooks in this repository, ensure you have the following packages installed:

- Python 3.x
- Jupyter Notebook
- Transformers
- PyTorch or TensorFlow
- Pandas
- Scikit-learn
- pdfplumber (for PDF extraction)
- Unsloth (for LLM fine-tuning)

You can install the required packages using pip:

```bash
pip install jupyter transformers torch pandas scikit-learn pdfplumber unsloth
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/DanieleCecca/NLP-project.git
   ```

2. Navigate to the project directory:

   ```bash
   cd NLP-project
   ```

3. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Open the desired notebook and follow the instructions provided within.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

