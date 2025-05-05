# JargonAI

**JargonAI** is a lightweight, end-to-end summarization pipeline for legal documents, built on Hugging Face’s FLAN-T5 model. It demonstrates data loading, preprocessing, model fine-tuning, and evaluation—all within a Colab-ready notebook.

## Features

- **Custom Legal Dataset**  
  Contains 60 human-written summaries of legal texts in `Corpus_all.csv` 
- **Pretrained Model**  
  Fine-tunes the `google/flan-t5-small` sequence-to-sequence model using PyTorch and the Transformers library.
- **Data Preprocessing**  
  • Tokenization with T5 tokenizer  
  • Train/validation split via `sklearn.model_selection.train_test_split`  
  • Batching using PyTorch `DataLoader`
- **Training Pipeline**  
  • Optimizer: `torch.optim.AdamW`  
  • GPU acceleration (Colab GPU recommended)  
  • Configurable hyperparameters (batch size, epochs)
- **Evaluation Metrics**  
  Computes **ROUGE** and **BERTScore** to quantify summary quality.
- **Interactive Notebook**  
  Colab-enabled `Summa_rizzer.ipynb` walks through each step, from dataset loading to metric visualization


