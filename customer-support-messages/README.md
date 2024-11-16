# Classification With LLM on Customer Support Messages Dataset

| Model                                  | Accuracy on Test Dataset |
|----------------------------------------|--------------------------|
| GPT-4O-Mini No Optimization            | 0.77                     |
| GPT-4O-Mini System Prompt Optimization | 0.81                     |
| GPT-4O-Mini Few-Shot Examples          | 0.85                     |
| GPT-4O-Mini Fine-Tuned                 | 0.99                     |
| BERT Zero-Shot                         | 0.06                     |
| BERT Fine-Tuned                        | 0.99                     |


## Dataset

We use a synthtic generated dataset: [bitext/Bitext-customer-support-llm-chatbot-training-dataset](https://huggingface.co/datasets/bitext/Bitext-customer-support-llm-chatbot-training-dataset)

- Notebook: [00-prepare-dataset.ipynb](00-prepare-dataset.ipynb)

## Auto optimize system prompt and for adding few shot examples.

We use adalflow to optimize the system prompt and few shot examples for classification task.
It can help accelerate to a better prompt for your classification task.

- Notebook: [01-auto-optimize-system-prompt-and-few-shot-for-classification.ipynb](01-auto-optimize-system-prompt-and-few-shot-for-classification.ipynb)

![01-auto-optimize-system-prompt-and-few-shot-for-classification.png](assets%2F01-auto-optimize-system-prompt-and-few-shot-for-classification.png)

## Fine-tune GPT-4o-mini

We fine-tune GPT-4o-mini on the training dataset generated in the first notebook 👆
We significantly improve the performance of the model on the classification task.

- Notebook: [02-fine-tune-gpt-4o-mini-for-classification.ipynb](02-fine-tune-gpt-4o-mini-for-classification.ipynb)

![02-fine-tune-gpt-4o-mini-for-classification.png](assets%2F02-fine-tune-gpt-4o-mini-for-classification.png)


## Fine-tune BERT

We fine-tune BERT on the training dataset generated in the first notebook 👆

[03-bert-as-benchmark.ipynb](03-bert-as-benchmark.ipynb)