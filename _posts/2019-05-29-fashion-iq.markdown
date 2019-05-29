---
title:  The Fashion IQ Dataset 
date:   2019-05-29
thumb:  /media/fashion-iq-teaser.png
paper_name: The Fashion IQ Dataset, Retrieving Images by Combining Side Information and Relative Natural Language Feedback
conf_name: Arxiv 2019 
paper_authors: Xiaoxiao Guo*, Hui Wu*, Yupeng Gao, Steven J. Rennie and Rogério S. Feris (* equal contribution) 
paper_pdf: https://arxiv.org/abs/tbd
---

### Overview

Fashion IQ is a new and novel dataset we contribute to the research community to facilitate research on natural language based interactive image retrieval. High fidelity interactive image retrieval, despite decades of research and many great
strides, remains a research challenge.  
We believe that our dataset can encourage further work on developing more natural and real-world applicable conversational shopping assistants.


<!--more-->

The images of fashion products that comprise our Fashion IQ dataset were originally sourced from Amazon.com. Similar to [5], we selected three categories of product items from the original [Amazon Review data](http://jmcauley.ucsd.edu/data/amazon/), specifically:Dresses, Tops&Tees, and Shirts. Additionally, for each image, we crawled Amazon.com and extracted corresponding product information, when available. We collected natural language based
user feedback, describing the differences between each target
product image and a single reference product image.
Note that these human-written relative descriptions are associated
with real-world context, including side information
derived from product descriptions and customer reviews.
This unique feature of the Fashion IQ dataset allows researchers
to investigate the advantages of natural language
feedback in conjunction with such contextual information,
which is often available in practice. The following figure shows the general pipelien of the dataset collection procedure. 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-collection.png">

<br/>
### Differences from Previous Datasets 

#### Fashion Datasets 


Below is the network architecture for our dialog manager, which consists of (1) a response encoder which
embeds the information from the current dialog turn to a visual-semantic representation; 
(2) a state tracker which receives the response representation and combines it with the history information; 
and (3) a candidate image generator, which samples an image to return to the user based 
on distances between the history representation to each database image.

<br/>
#### Image Retrieval with Natural Language Queries 
One challenge remains in order to train the dialog management in a goal-oriended, end-to-end fashion,
which is the lack of training data on user dialogs. The natural approach is to train the dialog manager in an online way
with human annotator in the loop. However, this procedure is prohibitively slow and expensive.
It takes about one minute to collect one set of dialog with 10 rounds of interactions. 
So 120k sets of training dialogs requires 2k hours of annotation effort.


To this end, we employed model-based reinforcement learning for training the dialog manager. The user model 
is based on a novel computer vision task: _relative image captioning_, which learns to describe prominant 
visual differences between two images using natural language. The trained relative captioner serves
as a proxy of human annotators and allows for efficient training of the dialog manager without costly annotation. 
We collected a dataset for relative image captioning and trained a show-attend-tell based captioner. 
We found that although there is a difference between the generated descriptions and human provided
descriptions, for the most cases, relative captioner is able to provide reasonable descriptions for any 
given pair of shoe images: 

<img alt="img" src="{{site.baseurl}}/media/relative_example.jpg">

<br/>
### Dataset Access and Download  
Below is a video showcasing an user interacting with the dialog manager. 
Code and dataset <a href="https://github.com/XiaoxiaoGuo/fashion-retrieval">are available here.</a> 

<a href="https://youtu.be/Iy-m_cxE5jg"><img alt="img" src="{{site.baseurl}}/media/fashion_video_snip.jpeg"></a>

### Dataset Statistics 
Basic statistics of
the resulting Fashion IQ dataset are summarized in Table 1.
In the following subsections, we provide additional details
regarding how we collected fashion attribute labels and the
relative captions.
Below is a video showcasing an user interacting with the dialog manager. 
Code and dataset <a href="https://github.com/XiaoxiaoGuo/fashion-retrieval">are available here.</a> 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-statistics.png">

### Fashion IQ Challenge v1 
Below is a video showcasing an user interacting with the dialog manager. 
Code and dataset <a href="https://github.com/XiaoxiaoGuo/fashion-retrieval">are available here.</a> 

<a href="https://youtu.be/Iy-m_cxE5jg"><img alt="img" src="{{site.baseurl}}/media/fashion_video_snip.jpeg"></a>

<br/>
### References

<p>
  [1] Xiaoxiao Guo*, Hui Wu*, Yupeng Gao, Steven J Rennie, and Rogerio S Feris. "Dialog-based Interactive Image Retrieval." NIPS 2018.(* equal contribution)
  [2] Xiaoxiao Guo*, Hui Wu*, Yu Cheng, Steven Rennie, and Rogerio Schmidt Feris. "Dialog-based Interactive Image Retrieval." NIPS 2018.(* equal contribution)
  [5] Z. Al-Halah, R. Stiefelhagen, and K. Grauman. "Fashion forward: Forecasting visual style in fashion". ICCV, 2017.
</p>

