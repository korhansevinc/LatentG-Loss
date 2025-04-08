# LatentG-Loss
Official Implementation of the LatentG Loss Paper


## Overview
This study presents a multi-stage approach to mental health classification by leveraging traditional machine learning algorithms, deep learning architectures, and transformer-based models. A novel data set was curated and utilized to evaluate the performance of various methods, starting with conventional classifiers and advancing through neural networks. To broaden the architectural scope, recurrent neural networks (RNNs) such as LSTM and GRU were also evaluated to explore their effectiveness in modeling sequential patterns in the data. Subsequently, transformer models such as BERT were fine-tuned to assess the impact of contextual embeddings in this domain. Beyond these baseline evaluations, the core contribution of this study lies in a novel training strategy involving a dual-model architecture composed of a teacher and a student network. Unlike standard distillation techniques, this method does not rely on soft label transfer; instead, it facilitates information flow through both the teacher model’s output and its latent representations by modifying the loss function. The experimental results highlight the effectiveness of each modeling stage and demonstrate that the proposed loss function and teacher-student interaction significantly enhance the model's learning capacity in mental health prediction tasks.

Model Chekcpoints, Datasets, Embeddings and Other util files can be found at : `https://drive.google.com/drive/folders/1SPyqW8wXPgBeK1i6CRVG9iV7sRSw_Lio?usp=sharing`

This repository includes:

- 📜 `train_textcnn_w_latentG_Loss.py` — Proposed Model architecture training script
- 📜 `train_*.py, finetune_*.py, test_*.py, sentiment_analysis.ipynb` — Training finetuning and evaluation scripts with proposed hyperparameters. 
- 📜 `DualArchitecture.py, RNNBasedModel.py, TextAutoEncoder.py, TextCNN.py, TextDataset.py, fit_mog_2_latent_descriptor.ipynb, fit_mog_2_latent_descriptor_dualarchitecture.ipynb, latentG_Loss.ipynb` — Configs, Utils and Architecture implementations 
- 📜 `tversky_loss.py , dice_loss.py` — Implementation of different loss functions  

- 📁 `drive folder` — Generated results, models, vectors, etc.