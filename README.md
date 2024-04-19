# AI PolicyChat
## Introduction Motivation:
Develop a fine-tuned Large Language Model that is capable of understanding and answering questions related to AI policy.

## Challenges:
- Provide insightful, contextually relevant responses
- Outperform the base Llama-2-7B model
- Effective Prompt Engineering
- Effective Fine-Tuning

## Methodology
- **Data Collection and Preparation:**
  - Policy Document subsets: International, US Government, Think-Tanks, Organizations, Forums
- **Prompting Techniques:**
  - Application to base and fine-tuned models
- **Fine-Tuning and Model Development:**
  - PEFT, Hyperparameter selection
- **Model Evaluation:**
  - Automatic and Human Evaluation

## Prompt Engineering Methods:
- Zero-Shot
- One-Shot
- Few-Shot
- Negative Prompting
- Chain-of-Thought Prompting

## Example Zero-Shot Prompting
### Input:
**Question:** List the most pressing topics regarding regulation of AI.
#### Base Output:
The most pressing topics regarding regulation of AI are:
1. Privacy and data protection: AI systems can collect and process vast amounts of personal data, which raises concerns about privacy and data protection.
2. Bias and discrimination: AI systems can perpetuate existing biases and discrimination, which can have a disproportionate impact on certain groups of people.
3. Accountability and transparency: AI systems can
#### Fine-Tuned Output:
- Defining AI accurately
- The role of AI in the future of work
- AI's impact on competition and pricing
- The role of AI in the next generation of digital platforms
- AI and the future of automation

## Example Chain-of-Thought Prompting
### Input:
**Question:** Why should international discourse take China's AI regulations seriously?</br>
**Prompt:**
1. First, summarize China's current state of affairs regarding regulation of information technology, data, and AI development.
2. Second, discuss China's most recent legislative changes regarding AI.
3. Then, state why other nations should pay close attention to China's new AI regulations.
#### Base Model Output:
- China's AI regulations are a good example of how to balance the need for innovation with the need for regulation.
#### Fine-Tuned Output:
China is a leading player in AI development and innovation, and its government is aware of this and wants to control this to benefit itself more efficiently. Other nations should pay close attention to China’s new AI regulations because they may serve as a template for how a government can control information and data more efficiently.
![image](https://github.com/Santhoshkumar-p/llama2-finetuning/assets/24734488/146585bc-50ff-4ece-a774-edf1a387918e)

## RAG & Fine-Tuning
- **RAG Framework:** LangChain
- **Embedding:** HuggingFace Embeddings(sentence-transformers/all-MiniLM-L6-v2)
- **Context Size:** 4 Chunks
- **Vector Store:** In-memory ChromaDB
- **PEFT:** QLoRA (r=8)
- **Quantization:** 4 bit
- **Epochs:** 10
<img width="938" alt="image" src="https://github.com/Santhoshkumar-p/llama2-finetuning/assets/24734488/83aa63d8-5b6b-4ad5-a5ce-5a62b9ba2ac1">


## Evaluation - Automatic Metrics
- BLEU
- ROUGE
- BERT Score

## Human Evaluation Criteria
- **Relevance:** Does the response address the prompt?
- **Informativeness:** Does the response provide accurate and relevant information?

