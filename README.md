# LLMs

You will find my toy projects on large language models (LLMs) in this page. Those contain in-depth instructions for several important tasks related to LLMs

1. Fine-tune Llama 2. The first project is to fine-tune Llama 2 to for travelling topics. The data collection on reddit with more than 8000 question-answer pairs is done by me and Phuoc Bui. In the notebook file, you will see a step-by-step guide to fine-tune any LLM with your own dataset.

2. Fine-tune Flan T5. The second project is to fine-tune and build a simple chatbot with Flan T5 small. The fine-tuning and response process is much faster than Llama 2, due to much less number of parameters. But it may take a lot of time to fine-tune Flan T5 small, because the answer is much less coherent than Llama 2.

3. Vector databases search for texts and images. The project aim to develop sematic search tools for texts and images. For dataset with text metadata, I use Sentence Transformer to embbed the text field. For images, I use ResNet to extract image features. I then save vectors in Qdrant vector databases to perform vector search. Before running the notebooks, you would need Docker desktop ready and you can pull and run the Qdrant service with the following command

```docker
docker pull qdrant/qdrant
docker run -p 6333:6333 qdrant/qdrant
