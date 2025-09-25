## **Exploring the Realm of Fine-Tuning LLMs and Embedding Models**

Recently haing been exploring the use of fine tuning LLMs and embedding models for NLP use cases. This repo is serves as a guide towards fine-tuning using methods such as;
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
- Fine tuning LLMs is computationally expensive but the fine tuning embeddings models is less expensive.
- You could fine-tuning an embedding model on your specific dataset to improve your RAG system as you may not need to fine tune a LLM.
- Fine tuning with prompts could replace the fine tuning LLMs due to the use of query-answer pairs thereby improving RAG retrieval.
- The Matryoshka embeddings fine tuning approach aids in the reduction of the embedding size especially for scaling purposes especially for mobile device as a large embedding space could affect latency during retrieval for RAG applications.
- LoRA adpaters aid in speeding fine tuning approaches in LLMs as you're not fine tuning the whole model weights but making subtle adjustments in the model weights by using two smaller matrices that approximate this larger matrix are fine-tuned.
- GRPO is a reinforcement approach that makes the model to reason before answering thereby making answers give by the model to be more concise. 

## **My Huggingface Repo**
[Link to all Huggingface models on this project](https://huggingface.co/DannyAI/models)