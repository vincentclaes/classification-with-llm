# Classification with LLM

This repo tries to perform text classification using an LLM and benchmark it versus BERT and others.

## Customer Support Messages Dataset

Predict if message is invoice,order,...
</br>More info: [customer-support-messages/](./customer-support-messages)

| Model                                  | Accuracy on Test Dataset |
|----------------------------------------|--------------------------|
| GPT-4O-Mini No Optimization            | 0.77                     |
| GPT-4O-Mini System Prompt Optimization | 0.81                     |
| GPT-4O-Mini Few-Shot Examples          | 0.85                     |
| GPT-4O-Mini Fine-Tuned                 | 0.99                     |
| BERT Zero-Shot                         | 0.06                     |
| BERT Fine-Tuned                        | 0.99                     |


## Yelp Dataset 

Predict the number of stars of a review. 
</br>More info: [yelp/](./yelp) folder.

| Model                                  | Accuracy on Test Dataset |
|----------------------------------------|--------------------------|
| GPT-4O-Mini System Prompt Optimization | 0.62                     |
| GPT-4O-Mini Few-Shot Examples          | 0.64                     |
| GPT-4O-Mini Fine-Tuned                 | 0.68                     |
| BERT Zero-Shot                         | 0.19                     |
| BERT Fine-Tuned                        | 0.30                     |
