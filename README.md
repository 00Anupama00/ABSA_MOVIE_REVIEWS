#  Aspect-Based Sentiment Analysis on IMDB Reviews

This project performs **Aspect-Based Sentiment Analysis (ABSA)** on IMDB movie reviews using a fine-tuned **BERT** model. Utilizing NLP techniques,this project identifies sentiment related to specific movie aspects (like acting, direction, storyline, etc.) and visualizes the confidence of predictions in a user-friendly Gradio interface.
# About this Project
🔹 1. Text Preprocessing & Tokenization - using BERT Tokenizer   
🔹 2. Aspect Extraction - using NLP methods like dependency parsing and named entity recognition (NER).   
🔹 3. Multi-Label Sentiment Classification - using pretrained BERT(Bidirectional Encoder Representations from Transformers)    
🔹 4. Sentiment Scoring -  probabilities of aspects in the given review are analyzed for aspect-sentiment prediction.

##  Features

-  Optimized for fast execution (Colab/GPU-ready)
-  Built with advanced transformer-based NLP models (BERT)
-  Multi-label aspect sentiment classification using BERT
-  Real-time sentiment analysis for aspects like acting, dialogues, storyline, etc.
-  Interactive visualization of aspect sentiments using matplotlib
-  Lightweight Gradio web interface

##  Aspects Analyzed

| Aspect           | Keywords                | Threshold |
|------------------|-------------------------|-----------|
| Acting           | act, perform            | 0.65      |
| Dialogues        | dialogue, script        | 0.60      |
| Storyline        | story, plot             | 0.55      |
| Characters       | character, role         | 0.50      |
| Cinematography   | camera, shot            | 0.45      |
| Visual Effects   | effect, vfx             | 0.40      |
| Direction        | director, vision        | 0.60      |

# Dataset Used
 ```bash
IMDB Dataset.csv --quiet
```

##  Installation

```bash
pip install transformers[torch] gradio pandas matplotlib 
```
# Run the Project
You can run the full project in Google Colab or locally (preferably with GPU).
The interface will launch a Gradio app:
```bash
iface.launch()
```
# Model Details
  - Pretrained BERT: bert-base-uncased
  - Multi-label classification head
  - Mixed precision training with AMP for performance
  - Optimized data loader and tokenizer usage


# Project Structure
```bash
├── IMDB Dataset.csv
├── aspect_sentiment_analysis.ipynb
├── temp_plot.png
├── README.md
```
# Language Used 
Python

# License
MIT License

# Acknowledgments
  * Hugging Face Transformers
  * Gradio
  * PyTorch
  * Kaggle IMDB Dataset


