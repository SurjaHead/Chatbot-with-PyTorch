<div align="center">
<h1 align="center">PyTorch Chatbot</h1>

  <p align="center">
    A simple chatbot implemented in PyTorch that responds to user input based on predefined intents.
  </p>
</div>

## Table of Contents

  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
      </ul>
    </li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#training-the-chatbot">Training the Chatbot</a></li>
        <li><a href="#running-the-chatbot">Running the Chatbot</a></li>
      </ul>
    </li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>

## About The Project

This project implements a basic chatbot using PyTorch. The chatbot is trained on a set of intents defined in `intents.json`.  It uses natural language processing techniques from the `nltk` library to understand user input and provide appropriate responses. The model is a simple neural network with three linear layers and ReLU activation functions.

### Key Features

- **Intent Recognition:**  Identifies the user's intent based on their input.
- **Customizable Intents:** The `intents.json` file can be easily modified to add new intents and responses.
- **Simple Neural Network:** Uses a basic neural network architecture for intent classification.
- **Tokenization and Stemming:** Employs `nltk` for tokenizing and stemming words to improve accuracy.
- **Bag of Words:** Represents sentences as bag of words for the neural network.

## Built With

- [Python](https://www.python.org/)
- [PyTorch](https://pytorch.org/)
- [NLTK](https://www.nltk.org/)
- [NumPy](https://numpy.org/)

## Getting Started

To get started with this project, follow the instructions below.

### Prerequisites

- Python 3.6 or higher
- PyTorch
- NLTK
- NumPy

Install the required packages using pip:

```sh
pip install torch nltk numpy
```

You also need to download the `punkt` tokenizer for NLTK:

```sh
python
import nltk
nltk.download('punkt')
```

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/surjahead/chatbot-with-pytorch.git
   ```
2. Navigate to the project directory:
   ```sh
   cd chatbot-with-pytorch
   ```

### Training the Chatbot

To train the chatbot, run the `train.py` script:

```sh
python train.py
```

This script will train the neural network using the data in `intents.json` and save the trained model to `data.pth`.

### Running the Chatbot

To run the chatbot, execute the `chat.py` script:

```sh
python chat.py
```

This will load the trained model and allow you to interact with the chatbot. Type `quit` to exit.

## Acknowledgments

- This README was created using [gitreadme.dev](https://gitreadme.dev) — an AI tool that looks at your entire codebase to instantly generate high-quality README files.
