# Fine-Tuning and Enhancing a Domain-Specific LLM for South African Food Recipe

This project demonstrates how to adapt a general-purpose language model (GPT-2 Medium) into a domain-specialized chatbot capable of answering questions about food, recipes, ingredients within the South Afriican Context. The approach integrates fine-tuning, retrieval-augmented generation (RAG), and reinforcement learning from human feedback (RLHF) to improve accuracy and usability.

## Objectives

- Customize a large language model with domain-specific data
- Leverage retrieval mechanisms to support grounded responses
- Implement a feedback loop for iterative improvement

## Base Model

- **GPT-2 Medium** (355M parameters)
- Pretrained on WebText
- Further trained on custom recipe and cooking corpus

## LLM Model Improvement

### Fine-Tuning

- Supervised fine-tuning on recipe instructions, ingredients, cooking Q&A Dataset
- Loss: CrossEntropyLoss on next-token prediction

### Retrieval-Augmented Generation (RAG)

- Dense passage retrieval (e.g., FAISS )
- External knowledge documents retrieved at query time

### Reinforcement Learning from Human Feedback (RLHF)

- Simulated user queries and rankings

## Applications

- **Recipe lookup:** Handles complex questions such as "How to make chicken curry?"
- **South African meals:** Suggests receipes for popular South African receipes
- **User personalization:** Adapts responses based on user preferences and history

<img width="612" height="459" alt="image" src="https://github.com/user-attachments/assets/6a6997c1-0f76-421e-acae-c505ae2e6202" />
