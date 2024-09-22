
# LLM Science Exam

This repository contains the implementation for the **LLM Science Exam** project, focusing on utilizing Large Language Models (LLMs) to answer science-based multiple-choice questions (MCQs). The project incorporates a DeBERTa-based model with an integrated Wikipedia-based context retrieval system, achieving an accuracy of 80%.

## Features

- **DeBERTa Integration**: Fine-tuned DeBERTa model for MCQ answering.
- **Context Retrieval**: Wikipedia article extraction and retrieval using FAISS indexing and the `all-MiniLM-L6-v2` model.
- **Preprocessing**: Efficient preprocessing of Wikipedia dumps to structure relevant context.


## Datasets

- **Wikipedia Dumps**: Downloaded and processed to provide relevant context for each MCQ.
- **Science MCQ Dataset**: Custom dataset of multiple-choice questions from various scientific domains.

## Model Architecture

- **DeBERTa**: A pre-trained transformer model fine-tuned for the task of MCQ answering.
- **FAISS**: Fast retrieval system for large-scale Wikipedia articles, ensuring low-latency context fetching.

## Results

- **Accuracy**: Achieved 80% accuracy on science-based MCQs with the help of context retrieval.
- **Benchmarking**: The model was evaluated on a well-structured test set to demonstrate performance.

## Installation

To set up the environment, run:

```bash
git clone https://github.com/heyyviv/LLM-science-exam.git
cd LLM-science-exam
pip install -r requirements.txt
```

## Usage

1. **Preprocess Wikipedia Data**: First, process the Wikipedia dumps.
   ```bash
   python preprocess_wikipedia.py
   ```

2. **Run the Model**: Execute the main script to answer MCQs.
   ```bash
   python run_model.py --input data/test_mcq.json
   ```

## Hugging Face Deployment

The project is deployed on Hugging Face Spaces. Check out the deployment here:
[Hugging Face Spaces - LLM Science Exam](https://huggingface.co/spaces/v1vu/image_captioning/tree/main)

## Running Notebooks on Kaggle

You can also run the notebooks and experiment with the model on Kaggle. Visit my Kaggle profile here:
[Kaggle Profile - heyviv](https://www.kaggle.com/heyviv)

## Future Work

- **Model Improvements**: Investigate additional model architectures like GPT-3 or PaLM.
- **Dataset Expansion**: Incorporate more diverse MCQ datasets from various scientific fields.
- **Contextual Retrieval**: Experiment with other knowledge bases for context retrieval.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with detailed explanations.

## License

This project is licensed under the MIT License.
