# README
## Introduction

I chose the dataset with consideration for the real world and the GPU limitations of my PC. The dataset consists of labor laws in PDF format, focusing on the United Arab Emirates (UAE). However, it can be applied to labor laws of any country. The dataset contains 196 documents. This dataset serves as a real-world application where users can ask questions about labor legislation, and the system will respond with relevant information.

## Model Selection

GPT (Generative Pre-trained Transformer) is the chosen model for this project due to its exceptional capabilities in question answering tasks. While my computer's limitations prevented training on large parameter models, GPT-Neo with 125 million parameters still provides significant power and flexibility for this application.
## Why GPT-Neo is a Better Option

- **Diverse and Human-like Response**: GPT models have the capacity to comprehend a wide range of patterns and provide responses that are human-like.

- **Comprehension of Context**: GPT models have a transformer design with attention mechanisms that enable them to provide pertinent responses in response to the context, even in complex scenarios. This allows them to have a profound grasp of context.

- **Adaptability**: GPT models can be improved for a variety of applications, such as chatbots, by fine-tuning them on certain datasets or tasks, such as answering questions.

- **Efficiency**: GPT models are a strong option for chatbot development since they show excellent performance in a variety of natural language processing tasks, including question answering.

## Limitations

- **Computational Resources**: A lot of memory and storage, together with high-performance GPUs or TPUs, are needed for training and optimizing GPT-Neo models.

- **Unable to Handle Unseen Scenarios**: GPT-Neo is limited in its ability to respond to situations to those that it has seen in training. Situations or subjects that differ greatly from the training set may be difficult for it to manage.

- **Dependency on Training Data**: The diversity and quality of the training data are crucial to GPT-Neo's performance. The training data's biases, errors, and limits may have a detrimental effect on the model's performance.

- **Creation of Incoherent Text**: Occasionally, GPT-Neo may produce text that is incomprehensible or illogical, particularly when creating lengthy sequences or responding to unclear instructions.

## Architectural Overview

### Transformer Blocks

A stack of transformer blocks makes up GPT-Neo. Usually, every transformer block consists of:

- **Multi-head Self-Attention Mechanism**: This technique enables the model to assess the relative weights of various words within the input string.
- **Feedforward Neural Network**: This network generates the final representations of the input sequence by processing the self-attention mechanism's output.
- **Layer Normalization**: Residual connections and layer normalization are extra elements that are introduced to training to stabilize it and make information flow across the network easier.

### Embedding Layers

Using embedding layers, GPT-Neo converts input tokens into continuous vector representations, or embeddings. These embeddings serve as the transformer blocks' initial input and capture the semantic meaning of the input tokens.

### Positional Encoding

Positional encoding is added to provide the model positional information because transformer architectures do not naturally comprehend the order of tokens in the input sequence.

### Tokenization and Vocabulary

The GPT-Neo model utilizes tokenization to transform input text into a sequence of tokens that the model can comprehend, while also utilizing a fixed-size vocabulary of tokens.

### Output Layer

Using the previous tokens as a guide, GPT-Neo's output layer forecasts the token that will come next in the sequence. This layer creates the probability distribution over the whole vocabulary during fine-tuning or generation, enabling the model to produce text that is both coherent and appropriate for the situation.
