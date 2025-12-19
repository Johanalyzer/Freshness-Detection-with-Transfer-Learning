# Produce Freshness Classification with Transfer Learning

This project studies **automated produce freshness classification** under **limited data conditions**, motivated by potential smart-fridge applications. Using a balanced dataset of fresh and rotten fruits and vegetables, we compare **ResNet-50** and **Vision Transformer (ViT-B/16)** under different training regimes.

## Approach
- 16-class classification (8 produce types × fresh/rotten)
- ImageNet-pretrained ResNet-50 and ViT-B/16
- Training regimes:
  - Frozen pretrained backbone
  - Fine-tuning of higher layers
  - Training from scratch
- Standard ImageNet preprocessing and data augmentation

## Key Findings
- **Transfer learning is essential** for reliable performance on small datasets
- **Fine-tuned models outperform frozen and scratch variants**
- **ResNet-50 achieves the highest accuracy and most stable training**
- Vision Transformers show **reduced stability and performance** under data scarcity, highlighting the importance of **inductive biases**

## Conclusion
The results indicate that **convolutional architectures remain the most robust choice** for freshness detection in constrained real-world settings such as smart fridges.

## Authors
Maxwell Bernard · Johan Schommartz  
Copenhagen Business School / IT University of Copenhagen

