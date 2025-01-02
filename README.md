# TiSASRec_ReChorus
@course MachineLearning 2024~2025


根据你提供的代码，以下是一个通用的 README 模板，概述了模型的主要功能及使用方式。
TiSASRec: Time Interval Aware Self-Attention for Sequential Recommendation
Overview
TiSASRec is a time-aware self-attention model for sequential recommendation, designed to capture the temporal patterns in user behavior. This model incorporates time intervals between interactions, allowing it to better model the sequential nature of user-item interactions in recommendation systems.
The architecture is based on a transformer-like model with time interval-aware self-attention layers. The model leverages both item embeddings and time interval embeddings to capture the influence of time on user preferences.
Reference
Title: "Time Interval Aware Self-Attention for Sequential Recommendation" 
Authors: Jiacheng Li et al., WSDM'2020. 
Installation
Make sure you have Python 3.x and the following dependencies installed:
PyTorch 
NumPy 
(Optional) pandas (if dataset handling is required) 
You can install the required packages using pip:
pip install torch numpy
Model Details
TiSASRec uses self-attention layers augmented with time interval embeddings to enhance sequential recommendation performance. The model can be customized with different hyperparameters, including embedding size, number of attention layers, and number of attention heads.
Key Features:
Time-Aware Self-Attention: The model takes time intervals into account, which helps in improving recommendations by considering the temporal relationships between user interactions. 
Transformer-based Architecture: The model uses multi-head attention with time-aware embeddings to capture long-range dependencies in the sequence. 
Customizable Hyperparameters: Various parameters such as embedding size, number of layers, and number of attention heads can be adjusted to fit the problem at hand. 
Usage
Command Line Arguments
The model can be run with the following arguments:
python main.py --model_name TiSASRec --emb_size 64 --num_layers 1 --num_heads 4 --lr 1e-4 --l2 1e-6 --history_max 20 --dataset 'Grocery_and_Gourmet_Food'
Arguments
