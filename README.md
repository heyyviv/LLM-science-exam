# LLM-science-exam

Kaggle LLM Science Exam Solution
This repository contains the solution for the Kaggle LLM (Language Learning Model) Science Exam competition. In this competition, participants were tasked with using LLMs to answer difficult science questions based on given contexts.

Overview
The solution utilizes various techniques from natural language processing (NLP) and deep learning to effectively tackle the challenge. Here's a breakdown of the approach:

Data Preparation:

The provided dataset containing science questions and corresponding contexts was preprocessed to extract relevant information.
Fine-tuning LLM:

A pre-trained LLM (Language Learning Model) was fine-tuned on the given dataset using the Hugging Face Transformers library.
The fine-tuning process involved training the model to understand the context and select the correct answer from multiple choices.
Embedding Retrieval:

To improve the model's performance, sentence embeddings were retrieved from relevant Wikipedia articles using the Sentence Transformers library.
These embeddings were used to enrich the contextual understanding of the model during inference.
Inference:

During inference, the fine-tuned LLM processed the input questions and contexts to generate predictions.
The predictions were refined by incorporating additional information from the retrieved embeddings, resulting in more accurate answers.
Submission Generation:

The final predictions were formatted according to the competition requirements and saved in a submission CSV file for evaluation.
Requirements
To replicate the solution, the following dependencies are required:

Python 3.x
Hugging Face Transformers
Sentence Transformers
Faiss (for efficient similarity search)
BlingFire (for efficient sentence boundary detection)
Other necessary libraries (specified in requirements.txt)
Usage
Clone the repository:

bash
Copy code
git clone https://github.com/heyviv/kaggle-llm-science-exam.git

link to notebooks
https://www.kaggle.com/code/heyviv/wikipedia-faiss-index-creation
https://www.kaggle.com/code/heyviv/llm-science-exam-p1
https://www.kaggle.com/code/heyviv/llm-scince-exam-part-2
https://www.kaggle.com/code/heyviv/llm-science-p3-submission

Install dependencies:

Copy code
pip install -r requirements.txt
Run the provided scripts:

bash
Copy code
python preprocess.py  # Data preprocessing
python train.py       # Fine-tune the LLM
python inference.py   # Generate predictions
Evaluate the model:

Submit the generated predictions to the Kaggle competition platform for evaluation.
Results
The solution achieved 0.78 on the Kaggle leaderboard, demonstrating its effectiveness in answering difficult science questions using LLMs.

Feel free to customize and expand upon this template based on your specific approach and results. Let me know if you need further assistance or clarification on any aspect!