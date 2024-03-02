# generate_chest_x_ray_images
Generative Adversarial Network (GAN) for Chest X-ray Image Generation, focusing on normal and pneumonia cases. Novel architecture addresses mode collapse and perceptual quality issues, ensuring balanced training and feature discovery by the discriminator. Conditional generation, MSE loss, and LayerNormalization used for improved results. 
For your Git repository, you can provide a detailed description of your project, highlighting its purpose, key features, and any unique aspects of your approach. Here's a sample description based on the work you've shared:

---

# Chest X-ray Image Generation using ACGAN

This project presents a novel approach to generating chest X-ray images for both normal subjects and patients with pneumonia. The goal was to address common challenges in Generative Adversarial Networks (GANs), such as mode collapse and perceptual quality, while ensuring the continuity of training and feature discovery by the discriminator.

**Key Features:**
- Conditional Generation: A conditional model was used for the GAN, where the discriminator determines the authenticity and pathological condition of the generated images.
- Balanced Training: The architecture ensures balanced training between the Generator and Discriminator, avoiding issues like mode collapse.
- Input Structure: The generator takes noise with a regular distribution along with the pathological condition to be classified, allowing for targeted image generation.
- Loss Function: Mean Squared Error (MSE) loss was used to improve perceptual quality and focus the generator on key health or pathological features.

**Approach:**
- The dataset included images of normal and pneumonia cases, with varying sample sizes per class.
- A smaller number of samples were passed to the GAN to avoid mode collapse and allow the generator to focus on key features.
- LayerNormalization was used instead of BatchNormalization to diversify generated images and prevent mode collapse.

**Results:**
- The proposed ACGAN architecture showed promising results in generating chest X-ray images.
- Further training and optimization could improve the accuracy and diversity of the generated images.

**Future Work:**
- Increase training time and sample diversity to further enhance the model's performance.
- Explore other loss functions and architectural tweaks to improve image quality and feature capturing.

---
