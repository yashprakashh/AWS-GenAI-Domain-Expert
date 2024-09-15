# AWS GenAI Domain Expert

## Fine-tuning Llama2 Large Language Model with Amazon SageMaker

### Project Overview

This project demonstrates how to fine-tune the Llama2 Large Language Model using Amazon SageMaker, with a particular focus on the financial domain. The key steps and outcomes are outlined below.

### 1. Evaluation of the Pre-trained Model

- **Notebook Instance Type:** `ml.t3.medium`
- **Amazon EC2 G5 Instance Type:** `ml.g5.2xlarge`

#### Steps:

1. **Deploy Llama2 Model on AWS SageMaker:**
   - Utilized the pre-trained Llama2 Text Generation Large Language Model.

2. **Assess Pre-trained Llama2 Model for Financial Domain Knowledge:**
   - **Input Example:** "The results are encouraging for aggressive investors."
   - **Model Output:** "For those inclined towards aggressive investment, the current stock trades at $31.40, marking a 45.6% increase from the 52-week low of $21.67 and a 66.4% rise from the 52-week high."

### 2. Fine-tuning the Large Language Model

- Fine-tuned the Llama2 Large Language Model using a dataset specific to the financial domain.

### 3. Evaluation of the Fine-tuned Model

- Deployed the fine-tuned Llama2 Model on AWS SageMaker.
- Evaluated the model on text generation tasks and its knowledge in the financial domain.

#### Steps:

1. **Domain-specific Input:**
   - "The results for the short in the money options > are shown in Table 1. Table The results for the short in the money options Strike Price (CAD) Exercise Price (CAD) Option Value (CAD) Exercise Price (USD) Option Value (USD) 0."

2. **Model Output:**
   - "The results for the short in the money options > [Cgenerated_text': ' were very impressive. The median result was 37% and the average result was 41%. The results for the out of the money options were very disappointing. The median result was -13% and the average result was -18%.1nThe results for the long in the money options were'}] "
