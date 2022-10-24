# CycleGAN-facial-bias
Imperfect EleGANce: Implications of CycleGANs Aggravating Biases on Facial Data


After I learned about computer vision in the COSMOS Program, I became captivated by artificial intelligence’s boundless potential in our modern world. However, because AI models require immense amounts of data to learn, I was curious about how they would react to existing biases in the training data. In the Pioneer Research Program with Dr. Suleyman Uludag's mentorship, I implemented CycleGAN, a popular data augmentation machine learning model, and empirically evaluated it for bias along the axes of skin tone and gender. 

After many in-depth literary reviews, I spent weeks collecting facial data, writing and executing code, and utilizing cloud GPUs to train the convolutional neural networks. Despite going down many rabbitholes, through precise statistical analysis I found that the model caused a significant exacerbation of bias against POC and women when stylizing faces to look like the faces of members of technology companies. Because these models are already used in healthcare and criminal justice, they could lead to adverse consequences against minority groups. 

# Introduction

To read more about our research, please see our full paper: [Imperfect EleGANce: Implications of CycleGANs Aggravating Biases on Facial Data](/research_paper.pdf)

Generative Adversarial Networks (GANs) have become a widely-used data aug- mentation technique for data-demanding deep learning models. In this paper, we demonstrate that CycleGAN, a popular image-to-image translation GAN, not only perpetuates, but aggravates biases along the axes of skin tone and gender when given a skewed training dataset of face images. While CycleGANs can synthetically gener- ate unique, unseen data samples, they are not as elegant as they appear due to mode collapse, which is when the generators collapse and are only able to produce a small variety of samples. Their use can lead to adverse effects when applied to real-world training datasets that are biased along latent dimensions. We empirically demon- strate that the GAN-generated dataset displayed a significant under-representation of non-white skin tones and feminine facial features when stylizing representative faces to look like the faces of members of technology companies. To demonstrate real-world implications of mode collapse in CycleGANs, we perform a case study on Snapchat’s CycleGAN-based “My Twin” filter, which disproportionately lightens the skin tone of women of color. This work acts to caution the use of GAN-based data augmentation methods in downstream tasks, which can lead to adverse consequences by further exacerbating biases against minority groups. It is critical that from an ethical standpoint, GAN practitioners for data augmentation ensure that both train- ing datasets and trained models are representative and diverse regarding sensitive features. We also recommend some future work.

# Test Model

To use and test the model, 
