## **Exploring the Realm of Fine-Tuning LLMs and Embedding Models**
I have recently been exploring the fine-tuning of LLMs and embedding models for NLP use cases. This repo serves as a guide to fine-tuning using methods such as:
- **LLMs**
    - LoRA (Low-Rank Adaptation)
    - QLoRA (Quantised Low-Rank Adaptation)
    - GRPO (Group Relative Policy Optimization; A reinforcement learning approach)
- **Embeddings**
    - Full Fine tuning
    - Adaptive layer
    - Adaptive Layer with Matryoshka Loss
    - Fine Tuning with Matryoshka Loss
    - Fine Tuning with Prompts
    - Fine Tuning with PEFT (Parameter-Efficient Fine-Tuning)

## **My Findings**
- Fine-tuning LLMs is computationally expensive, but fine-tuning embedding models is less so.
- You could fine-tune an embedding model on your specific dataset to improve your RAG system, as you may not need to fine-tune an LLM.
- Fine tuning with prompts could replace the fine tuning LLMs due to the use of query-answer pairs thereby improving RAG retrieval.
- The Matryoshka embedding fine-tuning approach helps reduce embedding size for scaling purposes, particularly on mobile devices, as a large embedding space can increase retrieval latency in RAG applications.
- LoRA adapters speed up fine-tuning in LLMs because you are not fine-tuning all the model weights. Instead, two smaller matrices that approximate the larger weight matrix are fine-tuned.
- GRPO is a reinforcement approach that encourages the model to reason before answering, resulting in more concise responses. 

## Important note
Focusing on the dataset format for each LLM and embedding model will be the **MOST IMPORTANT ASPECT OF FINE-TUNING**, as fine-tuning models has become easier with technological advancements..

## **My Huggingface Repo**
[Link to all Huggingface models on this project](https://huggingface.co/DannyAI/models)