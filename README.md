# Sentiment Analysis in Product Reviews

## About

This project aims to perform sentiment analysis on product reviews from a Brazilian e-commerce site. To achieve this, a BERT NLP Model was fine-tuned, to classify review texts as positive or negative.

The model was trained and evaluated using a [public Olist dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), available on Kaggle, containing thousands of real customer reviews.

## Features

1. **Data Preprocessing:** Cleaning and preparing review texts for the model.

2. **BERT Fine-tuning:** Fine-tuning the neuralmind/bert-base-portuguese-cased pre-trained model for the specific task of text classification.

3. **Performance Evaluation:** Analysis of model performance with industry standard metrics such as Accuracy and F1-Score.

4. **Inference Pipeline:** Creating a function to test the trained model with new sentences in real time.

## Results

The model achieved excellent performance on the test dataset, demonstrating high generalization ability to classify the sentiment of texts it has never seen before.

| Accuracy | F1-Score | Validation Loss |
|----------|----------|-----------------|
| 93.7% | 93.7% | 0.192 |

```console
Resultados da Avaliação Final:
{'eval_loss': 0.19226007163524628, 'eval_accuracy': 0.937, 'eval_f1': 0.9369027269598926, 'eval_runtime': 6.3185, 'eval_samples_per_second': 316.531, 'eval_steps_per_second': 19.783, 'epoch': 3.0}
Device set to use cuda:0
Texto: 'Adorei o produto, chegou muito rápido e é de ótima qualidade!'
Resultado: [{'label': 'LABEL_1', 'score': 0.9961045980453491}]
Texto: 'Péssima experiência, o produto veio quebrado e a entrega demorou semanas.'
Resultado: [{'label': 'LABEL_0', 'score': 0.9972532391548157}]
```

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

## Contact

Leonardo Santos - <leorsantos2003@gmail.com>
