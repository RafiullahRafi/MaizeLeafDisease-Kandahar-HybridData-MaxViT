# Maize Leaf Disease Classification under Real Agricultural Conditions Using CNN, Vision Transformer, and MaxViT Architectures

## Experimental Results

The performance of multiple deep learning architectures was evaluated for maize leaf disease classification using a field-based and hybrid dataset. The experiments were conducted under different training configurations, including variations in batch size, input image resolution, and gradient accumulation. Model performance was assessed using Accuracy, Precision, Recall, and F1-score metrics. The comparative results demonstrate the effectiveness of transformer-based and hybrid CNN-transformer models in capturing disease-related visual patterns under real-field conditions.

## Utilized Models
The following deep learning models were implemented and evaluated:

- EfficientNet (B5, B6, and B7)
- Vision Transformer (ViT)
- MaxViT (Tiny, Small, and Base)

All models were trained using PyTorch and TIMM with customized training configurations.


### Model Performance Comparison

| Model                   | Batch Size | Image Size | Accumulation Gradient | Accuracy | Precision | Recall | F1-score |
|-------------------------|------------|------------|------------------------|----------|-----------|--------|----------|
| EfficientNet-B5         |     8      |    456     |           1            | 0.94     | 0.9251    | 0.9329 | 0.9263   |
| EfficientNet-B6         |     4      |    528     |           2            | 0.96     | 0.9583    | 0.9500 | 0.9512   |
| EfficientNet-B7         |     2      |    600     |           4            | 0.97     | 0.9658    | 0.9748 | 0.9700   |
| Vision Transformer (ViT)|     16     |    224     |           –            | 0.97     | 0.9658    | 0.9748 | 0.9700   |
| MaxViT-tiny-rw-224      |     32     |    224     |          –             | 0.97     | 0.9741    | 0.9667 | 0.9692   |
| MaxViT-small-tf-224     |     16     |    224     |          –             | 0.95     | 0.9440    | 0.9333 | 0.9331   |
| MaxViT-base-tf-224      |     8     |    224     |          –             | 0.92     | 0.9023    | 0.9243 | 0.9110   |



## Dataset
- You can download or open the model notebook using the links below:

-- [🚀 Open in Google Colab](https://colab.research.google.com/github/RafiullahRafi/MaizeLeafDisease-Kandahar-HybridData-MaxViT/blob/main/MaxViT_model_on_with_and_without_background_data.ipynb)

-- [Download dataset here](https://github.com/RafiullahRafi/MaizeLeafDisease-Kandahar-HybridData-MaxViT/blame/main/Kdr_field_Dataset.zip)


## Key Findings
- EfficientNet models showed improved performance with increased depth and image resolution, with EfficientNet-B7 achieving the highest recall and F1-score among CNN-based models.
- The Vision Transformer (ViT) delivered comparable results using smaller input images, demonstrating the effectiveness of self-attention for capturing global features.
- MaxViT models provided stable and balanced performance, with MaxViT-tiny-rw-224 achieving the highest precision, while larger variants showed no further improvement.
- Overall, transformer-based and hybrid architectures outperformed purely CNN-based models on the maize leaf disease dataset.


## Author
Rafiullah Rafi  
Department of Agricultural Engineering, Afghanisatan National Agricultural Sciences and Technology University(ANASTU), Kandahar, Afghanistan  
Email: r.rafi@anastu.edu.af
