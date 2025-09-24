# **Monet Painting with CycleGAN**

This repository contains a project to generate Monet-style paintings from photographs using a Generative Adversarial Network (GAN), specifically a CycleGAN architecture. The goal was to learn and replicate the distinctive artistic style of Claude Monet—his color palette, brush strokes, and use of light—to perform an artistic style transfer.

## **Model Architecture**

The model is built on a U-Net-based generator and a discriminator, following a tutorial-based approach that was enhanced with improved documentation, code modernization, and support for both Kaggle and Google Colab environments. The project successfully demonstrates the process of training a GAN for image-to-image translation.

## **Key Results**

The model's performance was evaluated based on a public score, where a lower score indicates a more successful style transfer. The primary hyperparameter tuned was the number of training epochs. The results showed a clear and direct correlation between increased training time and improved performance.

| Run Number | Epochs | Time    | Public Score |
|------------|--------|---------|--------------|
| 1          | 5      | 14 min  | 85.19853     |
| 2          | 10     | 17 min  | 75.73469     |
| 3          | 15     | 21 min  | 74.69851     |
| 4          | 20     | 25 min  | 64.63606     |
| 5          | 40     | 41 min  | 56.21900     |

The baseline model, trained for only 5 epochs, performed poorly. However, the best model, trained for 40 epochs, achieved a score of 56.21900. A significant improvement was achieved with more training and a strong ability to capture Monet's artistic essence was exibited.

## **Conclusion**

This project successfully implemented a CycleGAN for artistic style transfer, transforming standard photographs into compelling Monet-style artworks. The experiments confirm that sufficient training is critical for the model to learn the nuances of a complex artistic style. The final model is capable of generating thousands of convincing images that reflect Monet's iconic aesthetic.
