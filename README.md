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

## Results

The results obtained during experimentation are stored in the `results/` folder.

- `loss_comparison.png`: Training and validation loss comparison between the baseline LSTM model and the Transformer-based model.
- `cider_comparison.png`: CIDEr score comparison across epochs.
- `rouge_comparison.png`: ROUGE-L score comparison for long video sequences.

These figures are generated directly from the code in `Experiment_notebook.ipynb`.

## References

[1] Vaswani, A. et al. (2017). *Attention Is All You Need*. Advances in Neural Information Processing Systems (NeurIPS).

[2] Hochreiter, S. and Schmidhuber, J. (1997). *Long Short-Term Memory*. Neural Computation.

[3] Simonyan, K. and Zisserman, A. (2014). *Very Deep Convolutional Networks for Large-Scale Image Recognition*. arXiv preprint arXiv:1409.1556.

[4] Hori, C. et al. (2018). *Attention-based Multimodal Video Description*. IEEE International Conference on Computer Vision (ICCV).

[5] Papineni, K. et al. (2002). *BLEU: a Method for Automatic Evaluation of Machine Translation*. ACL.

