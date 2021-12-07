# ArtGan

General Idea:
Translating real images to Realism art style images. This art style dates back to the 17th century and there is no image-to-image pair data available to train traditional networks, So here I am implementing ideas expressed in the paper ***Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks (https://arxiv.org/pdf/1703.10593v7.pdf)*** and creating a GAN to transfer real Image to realism art style image, a bi-product of this implementation will also be capable to convert Realism art style images to somewhat real photo.  

I’m using Realism image folder from dataset ***https://github.com/cs-chan/ArtGAN/tree/master/WikiArt%20Dataset***  
***All the datset used is probably copyrighted, please check Copyright & privacy policy of WikiArt for more information (https://www.wikiart.org/en/terms-of-use).***
***Only can be used for academic and research.***   

________________________   
## Sample from dataset:  

![isaac-levitan_train-on-the-way](https://user-images.githubusercontent.com/14234116/140399395-df9be7ba-0ca4-497b-b975-254bb5197cb2.jpg)   
   
![vasily-surikov_portrait-of-natalia-f-matveeva-1909](https://user-images.githubusercontent.com/14234116/140399421-c5dbfaa6-6f7e-454b-a8b9-3ff9cf9b451a.jpg)   
   
![charles-francois-daubigny_sand-quarries-near-valmondois](https://user-images.githubusercontent.com/14234116/140399597-5dc3e9a7-a233-4629-93d8-23a89b428375.jpg) 

_________________________
## Proposed Evaluation   

Because of the above-mentioned issues, I’ll be deviating from baseline and evaluation metrics from the base paper and instead will be using a likeness score as   defined in the paper A Novel Measure to Evaluate Generative Adversarial Networks Based on Direct Analysis of Generated Images (https://arxiv.org/pdf/2002.12345.pdf)  which defines a likeness score as a combination of Creativity, Inheritance, and Diversity.
