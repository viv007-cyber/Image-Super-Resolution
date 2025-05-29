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
![image](https://github.com/user-attachments/assets/3b44f276-fb42-4a4e-a92d-5a4a0600d75a)
