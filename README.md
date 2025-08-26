# My Own GPT: A Character-Level GPT Implementation

## Overview

This project is a complete implementation of a GPT (Generative Pre-trained Transformer) model from scratch, built using PyTorch. It is designed to understand the inner workings of Large Language Models by building every core component, from the basic bigram model to the full transformer block with self-attention.

This project is based on the phenomenal "Let's build GPT" by Andrej Karpathy.

## Key Features

- **Built from Scratch:** Core components like the self-attention mechanism, multi-head attention, and transformer blocks are implemented from the ground up.
- **Progressive Learning:** Starts with a simple Bigram model as a baseline before implementing the full GPT architecture.
- **Training & Validation:** Includes proper training and validation loops to monitor model performance and prevent overfitting.
- **Text Generation:** The trained model can generate new text character by character based on the provided training data.

## How to Run

1.  **Clone the repository:**

2.  **Create a virtual environment and install dependencies:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

    _(Note: You will need to update your `requirements.txt` to include `torch` and `jupyter`)_

3.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook myowngpt.ipynb
    ```

## Results & Sample Output

After training the GPT model for 5000 iterations, over a whopping 10.81123 M parameters,the validation loss was successfully reduced to approximately 1.2. The model learned to generate text that mimics the structure of the input data.

The output below demonstrates that the model successfully learned:

- **Word Structure:** Grouping characters into word-like units separated by spaces.
- **Punctuation and Capitalization:** Using quotes for dialogue, periods, commas, and capital letters correctly.
- **Vocabulary:** Spelling some words from the training data, like "Watson" and "Holmes".

**Sample Generated Text:**

> "What kning on I am to resore eye cams to 'nexter feelock of her in the pizle, Watson not the clooke in we to same to... He dridchy and the cruling brom as eflecter."
