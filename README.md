# Llama3 Multilingual Fine-Tuning Project

## Introduction
Based on the [blog post]([https://www.google.com](https://medium.com/@ccibeekeoc42/unlocking-low-resource-language-understanding-enhancing-translation-with-llama-3-fine-tuning-df8f1d04d206)), this repository hosts the fine-tuning framework for Llama3, an open-source, multilingual model trained to improve language understanding across underrepresented languages, with a focus on Yoruba, Igbo, and English. Building on the innovative architecture and features of Llama2, Llama3 integrates advanced techniques like RMS Pre-Normalization, Rotary Positional Embeddings, KV-Cache, Grouped Query Attention, and more to enhance performance and efficiency.

## Model Overview
Llama3 extends Llama2’s capabilities by including:
- **RMS Pre-Normalization**: Optimizes the efficiency of neural network training by scaling input features using their root mean square, thus accelerating convergence.
- **Rotary Positional Embeddings (RoPE)**: Enhances context understanding by using relative distances within token sequences, which is crucial for processing longer texts.
- **KV-Cache**: Reduces redundant computations during inference, significantly speeding up the processing while managing memory usage effectively.
- **Grouped Query Attention**: Minimizes memory footprint and accelerates inference times by grouping queries before computing attention.

## Installation

### Prerequisites
- Python 3.8+
- PyTorch 1.8+
- Transformers 4.8+
- Datasets library from Hugging Face

### Setup
Clone this repository and install the required packages:
```bash
git clone https://github.com/yourusername/llama3-finetuning.git
cd llama3-finetuning
pip install -r requirements.txt
```

## Usage
To Understand and ruuse/ replicate this work on your dataset, follow the steps outlined below:

### Data Preparation
Refer the the file in this repo called "Llama2_Dataset_Prep.ipynb" and adapt it to your own data as needed. Ensure your dataset is formatted correctly, following the structure necessary for effective training. 

### Model Training (Fine Tunning)
Refer the the file in this repo called "Llama3_8b_SFT_Finetune.ipynb" Run the fine-tuning process with adapted to your needs.

### Inference/ Evaluation
Refer the the file in this repo called "Llama2_SFT_Inference.ipynb" Run the fine-tuning process with adapted to your needs. Evaluate the fine-tuned model to understand its performance and improvements:

## Contributing
Contributions to this project are welcome! You can contribute in several ways:
1. **Issues**: Submit issues for any bugs encountered or enhancements.
2. **Pull Requests**: Submit PRs for bug fixes or new features, following the pull request guidelines provided.
3. **Documentation**: Enhancements to documentation or new examples are always appreciated.

## License
This project is licensed under the terms of the MIT license (lol I dont know what this means).

## Citation
If you use this framework or the Llama3 model in your research, please cite it as follows:
```bibtex
@misc{llama3_2024,
  title={Llama3 Multilingual Fine-Tuning},
  author={Christopher Ibe & Okezie Okoye},
  year={2024},
  howpublished={\url{https://github.com/ccibeekeoc42/llama3-finetuning}},
}
```
