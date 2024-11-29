# *Hate Speech Detection in Code-Mixed Indo-Aryan Languages*

## *Problem Statement*  
Languages are crucial in communication, culture, and social interactions, particularly in multilingual regions such as South Asia. Hindi and Bengali, two of the world’s most spoken Indo-Aryan languages, are central to this landscape.  
- *Hindi:* 609.5 million speakers, 4th most spoken language globally.  
- *Bengali:* 272 million speakers, 7th most spoken language globally.  

As online platforms grow, these languages have evolved into code-mixed forms like *Hinglish (Hindi-English)* and *Banglish (Bengali-English)*. This blend, while reflecting cultural and practical factors, also leads to increased hate speech in online spaces. The informal and dynamic nature of these languages presents unique detection challenges. This project aims to develop robust methods to detect hate speech in Hinglish and Banglish, contributing to safer digital environments and advancing multilingual NLP research.

---

## *Project Overview*  
This project compares the performance of hate speech detection models across Hinglish and Banglish using *BERT-based architectures*, emphasizing the linguistic complexities of multilingual code-mixed environments.  



---

## *Current Progress*  
- *Hinglish Model Accuracy:* 72%  
- *Banglish Model Accuracy:* 75%  
- Built using bert-base-multilingual-cased, a pre-trained model supporting over 100 languages.

---

## *Key Techniques and Methodology*  

### *1. Data Preprocessing*  
- *Cleaning:* Lowercasing, removing special characters, and eliminating URLs.  
- *Tokenization:* BERT's *WordPiece Tokenizer* handles sub-word units effectively.  
- *Attention Masking:* Differentiates between meaningful tokens (1) and padding tokens (0).  

### *2. Model Architecture*  
- *TFBertModel:* Extracts contextual embeddings from input text.  
- *Classification Layer:* Fully connected with a sigmoid activation function to classify text as hate speech or non-hate speech.  

### *3. Training Details*  
- *Loss Function:* Binary Cross-Entropy.  
- *Optimizer:* Adam, with a learning rate of 1e-5.  
- *Validation Strategy:* Evaluates accuracy and loss metrics on the validation set.  

### *4. Evaluation Metrics*  
- *Accuracy:* Primary performance metric.  
- *Classification Report:* Includes precision, recall, and F1-score for both classes.  

---

## *Preliminary Insights*  
- *Banglish Model*: Outperforms Hinglish due to a less noisy dataset and better linguistic structure.  
- Effective preprocessing and tokenization techniques are critical to capture the intricate patterns in code-mixed languages.

---

## *Future Directions*  
- *Hyperparameter Tuning:* To optimize model performance.  
- *Architecture Exploration:* Experimenting with *LSTM + BERT embeddings* and *MConv-LSTM + BERT embeddings*.  
- *Comparative Analysis:* To refine approaches and optimize detection capabilities.  

---



![Architecture](https://github.com/user-attachments/assets/19438379-7f35-4513-9c72-27779bf18858)
