# Investigating Collapse on RL Fine-Tuning Data Distribution

## Overview

This project explores the impact of fine-tuning data distribution on the performance of models trained with Reinforcement Learning from Human Feedback (RLHF). It aims to understand how different linguistic features in the fine-tuning dataset influence the model's ability to generate diverse and accurate outputs.

## Team

- Marc Baumholz - marc.baumholz@student.uni-tuebingen.de
- Meike Kriegeskorte - meike.kriegeskorte@student.uni-tuebingen.de
- Line Abele - line.abele@student.uni-tuebingen.de

## Abstract

Large Language Models (LLMs) are powerful tools with wide applications, yet they often struggle to capture the full spectrum of diversity present in their training datasets. This study investigates the relationship between fine-tuning data distribution and model behavior, particularly focusing on the model's adaptability across varied linguistic contexts. Through rigorous analysis and evaluation, we reveal insights into the model's generalization capabilities and its resistance to overfitting tendencies.

## Methodology

Our methodology includes linguistic analysis of the training and test datasets, focusing on sentence length, sentiment scores, syntactic structure (via POS tagging), and lemmatization. We evaluated the model's performance using both intuitive human responses and a sophisticated reward model. The goal was to test the hypothesis that a model might overfit to properties dominant in the fine-tuning dataset, affecting its performance across different inputs.

## Findings

Our study found no significant overfitting towards features dominant in the fine-tuning dataset. The model exhibited robustness, with human quality judgments closely aligning with the reward model's evaluations across various inputs. This suggests that RLHF-trained models can effectively capture linguistic diversity without bias towards specific linguistic features.

The linguistic analysis of the training set is a large *csv* and can be found [here](https://drive.google.com/file/d/1qYGJKI-Q3F6Bl9PZMnWVg5C9KrvQ9lXd/view?usp=sharing).

## Discussion and Conclusion

The findings challenge preconceived notions about the predictability of model performance based on specific linguistic features of the training data. This contributes to the discourse on dataset development and evaluation for RLHF, emphasizing the need for nuanced understanding and innovative evaluation methods.

## Acknowledgements

We want to thank the developer of the spaCy-cleaner for the code on GitHub that we could adapt for our linguistic analysis 6. We also want to thank Polina Tsvilodub for the project idea, her advice and support, and for running the reward model.

## How to Use

1. **Installation**: Ensure you have Python 3.x installed. Clone the repository and install dependencies from `requirements.txt`.
2. **Running Analyses**: Navigate to the project directory and execute the scripts as described in the documentation. Make sure that the data is located in the corresponding folder.
3. **Evaluating Model Performance**: Use the provided notebooks to replicate our evaluation process or to analyze new datasets.

## Contributing

We welcome contributions from the community, whether it's improving the code, addressing issues, or extending the research. Please feel free to fork the repository and submit pull requests.
