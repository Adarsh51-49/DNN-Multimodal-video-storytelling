# Improving Long-Range Multimodal Video Storytelling Using Transformer-Based Architectures

## Module
Deep Neural Networks and Learning Systems (55-710365)

## Project Overview
This project focuses on improving multimodal video storytelling by addressing the limitations of traditional CNN–LSTM architectures when handling long video sequences. Recurrent models often struggle with long-range dependencies, leading to fragmented narrative generation.

To overcome this issue, this project proposes a Transformer-based architecture that leverages self-attention mechanisms to better capture long-term temporal relationships across visual and textual modalities.

## Dataset
The StoryReasoning Dataset is used, consisting of sequential image–text pairs designed for visual story understanding and grounded narrative generation. A strict video-level split is applied to avoid data leakage.

- Training: 80%
- Validation: 10%
- Test: 10%

## Baseline and Proposed Model
**Baseline:** VGG16 + LSTM  
**Proposed:** Vision Transformer (ViT) + Transformer Decoder with Self-Attention

## Evaluation
Performance is evaluated using CIDEr, ROUGE-L, and qualitative narrative flow analysis. Validation plots are used to compare baseline and proposed architectures.

## Conclusion
Results show that Transformer-based architectures provide improved long-range temporal reasoning and more coherent narrative generation compared to LSTM-based models.