# Image-Super-Resolution
Image super-resolution (SR) aims to enhance low-resolution images to high-resolution quality. This paper explores the effectiveness of ESRGAN (Enhanced Super-Resolution Generative Adversarial Network) on a dataset of 80 paired low- and high-resolution images, comparing its performance to benchmark models on a test set.

ESRGAN utilizes Residual-in-Residual Dense Blocks (RRDB)—excluding batch normalization—for efficient feature learning. It incorporates a relativistic GAN, where the discriminator estimates the relative realness of images instead of absolute values. The model optimizes a perceptual loss composed of adversarial loss (driving outputs toward the natural image manifold) and content loss (prioritizing perceptual similarity over pixel-wise accuracy).

Despite a limited training dataset, fine-tuning allowed ESRGAN to outperform benchmarks, generating more realistic textures and higher-quality outputs for single-image super-resolution.


I propose 2 results one with high perceptual quality but low PSNR and SSIM value and one with high pixel accuracy and low perceptual quality


Training through MSE optimization

![image](https://github.com/user-attachments/assets/3b44f276-fb42-4a4e-a92d-5a4a0600d75a)

Training through Perceptual loss optimization

<img width="700" alt="perceptual" src="https://github.com/user-attachments/assets/f1085e13-8210-4274-aace-c3b10a00ed3d" />


### Results when optimzing mse loss
Test PSNR: 28.2055
Test SSIM: 0.7394
Test LPIPS:0.2205



<img width="451" alt="Capture" src="https://github.com/user-attachments/assets/4f7fc105-9fa1-4c3b-8616-6fed51b5c517" />







### Results when optimizing perceptual loss
Test PSNR: 27.3911
Test SSIM: 0.7073
Test LPIPS: 0.1257


<img width="468" alt="Capture2" src="https://github.com/user-attachments/assets/5f475a68-0747-403e-afa8-3d52b00c566e" />




## Evaluation through other models
Our model has performed very well as compared to the standard models used in this field and can produce even better results.


### OriginalESRGAN:
Test PSNR: 27.3863
Test SSIM: 0.7033
Test LPIPS: 0.1972


### SRCNN
TestPSNR: 27.5452
Test SSIM: 0.7262



### Bicubic:
TestPSNR : 25.7640
Test SSIM : 0.6608


Hello!






