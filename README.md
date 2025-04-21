DDMSNet for Fog Removal
This project adapts the Deep Dense Multi-Scale Network (DDMSNet), originally designed for snow removal, to effectively reduce fog in images. We incorporated enhanced depth attention mechanisms and residual dense blocks to improve image clarity while preserving detail. The model was trained and evaluated on the Foggy Cityscapes dataset.
Overview
- Goal: Improve visibility in foggy images for applications such as autonomous driving and surveillance.
- Approach: Modify DDMSNet with:
  • Enhanced depth attention
  • Residual dense blocks (RDBs)
  • Semantic segmentation for detail preservation
Techniques Used
- Deep Convolutional Neural Networks (CNNs)
- Multi-scale residual learning
- Depth estimation and perceptual loss
- Semantic segmentation
- PyTorch for model development and training
Results
- Dataset: Foggy Cityscapes
- Metrics:
  • PSNR: 14.8 dB (Validation)
  • SSIM: 0.589
- Qualitative: Improved image clarity, contrast, and color fidelity in foggy conditions
File Structure
• depth_attention_model.py – Depth attention module
• residual_dense_block.py – Residual dense blocks
• model.py – Full architecture with segmentation
• train.py – Training script
• train_data.py – Dataset and data loader
• perceptual.py – Loss functions
• test.py – Model evaluation
• test_one.py – Single image test
Future Work
- Explore more advanced depth estimation models
- Improve fog removal under extremely dense fog
- Test with real-world foggy images
References
- DDMSNet for Snow Removal: https://github.com/HDCVLab/Deep-Dense-Multi-scale-Network-for-Snow-Removal.git
- Cityscapes Dataset: https://www.cityscapes-dataset.com/
