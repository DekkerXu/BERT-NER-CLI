# BERT_NER_CLI Step by Step Guide

Before started, would like to appreciate for [Google Research Team](https://github.com/google-research) and [@Kaiyinzhou's](https://github.com/kyzhouhzau) previous work at [here](https://github.com/kyzhouhzau/BERT-NER).

- [Environment](#environment)
- [Folder structure](#Folder-structure)
- [Fine-Tune model](#Fine-Tune-model)
- [Training with GCP GPU/TPU](#Training-with-GCP-GPU/TPU)
- [Evaluating](#evaluating)
- [Predicting](#predicting)

## Environment
* Python 3.5+
* Tensorflow 1.11+

## Folder structure
| Item             | Desc                |
| ------------------ |:------------------:|
| NERdata      | training / evaluating dataset |
| bert      | bert code download from [here](https://github.com/google-research/bert)      |
| bert_ner.py | training code      |
| ner_predict.py | predict code      |
| predict_cli.py | simple command line program for testing purpose |

## Fine-Tune model


## Training with GCP GPU/TPU
I found this pretty detailed [instructions](https://medium.com/deep-learning-turkey/google-colab-free-gpu-tutorial-e113627b9f5d) of how to deploy code, mount folders and execute .py files with Google Colab and utilizing their FREE TPU/GPU capabilities.

BERT-Base, Uncased or BERT-Large, Uncased need to be unzipped and upload to your Google Drive folder and be mounted.

I used Colab GPU (K80) fine-tuning the model, took me around 30 mins.

## Evaluating
A evaluation script can be found [here](https://github.com/kyzhouhzau/BERT-NER).

## Predicting
A simple command line program was provided here for testing purpose. Simply run
```sh
python predict_cli.py
```
The program will firstly load the model and waiting for inputs.


