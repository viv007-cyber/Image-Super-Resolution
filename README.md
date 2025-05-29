# Image-Super-Resolution
Advancements in computer vision are progressively increasing day by day, and so is the
progress made in one of its applications which is Image super-resolution, which involves
enhancing resolution of low quality images to produce high resolution images. Several
attempts have-made in this field to produce remarkable results on low resolution
images.
This paper focuses on employing ESRGAN(Enhanced super resolution generative
adversarial network) on a training dataset which contains 80 sets of low resolution
images and their corresponding high resolution images and comparing its results with
other benchmark models on a testing dataset. The model employs the usage of the
Residual-in-Residual Dense Block (RRDB) without batch normalization as the basic
network building unit.Moreover, relativistic GAN lets the discriminator predict relative
realness instead of the absolute value. It proposes a perceptual loss function which
consists of an adversarial loss and a content loss. The adversarial loss pushes our
solution to the natural image manifold using a discriminator network that is trained to
differentiate between the super-resolved images and original photo-realistic images. In
addition, content loss is motivated by perceptual similarity instead of similarity in pixel
space.
The main issue that plagued this task was the size of the training dataset but, through
the use of effective fine tuning the model was able to produce results that bettered the
results produced by the benchmark models, thereby generating realistic textures during
single image super-resolution.


I propose 2 results one with high perceptual quality but low PSNR and SSIM value and one with high pixel accuracy and low perceptual quality


Training through MSE optimization

![image](https://github.com/user-attachments/assets/3b44f276-fb42-4a4e-a92d-5a4a0600d75a)

Training through Perceptual loss optimization

<img width="700" alt="perceptual" src="https://github.com/user-attachments/assets/f1085e13-8210-4274-aace-c3b10a00ed3d" />


# Results when optimzing mse loss
Test PSNR: 28.2055
Test SSIM: 0.7394
Test LPIPS:0.2205



<img width="451" alt="Capture" src="https://github.com/user-attachments/assets/4f7fc105-9fa1-4c3b-8616-6fed51b5c517" />







# Results when optimizing perceptual loss
Test PSNR: 27.3911
Test SSIM: 0.7073
Test LPIPS: 0.1257


<img width="468" alt="Capture2" src="https://github.com/user-attachments/assets/5f475a68-0747-403e-afa8-3d52b00c566e" />


Evaluation through other models
Our model has performed very well as compared to the standard models used in this field and can produce even better results.


OriginalESRGAN:
Test PSNR: 27.3863
Test SSIM: 0.7033
Test LPIPS: 0.1972

SRCNN
TestPSNR: 27.5452

Test SSIM: 0.7262

 Bicubic:
TestPSNR : 25.7640
Test SSIM : 0.6608









