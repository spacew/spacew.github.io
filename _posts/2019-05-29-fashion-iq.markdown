---
title:  The Fashion IQ Dataset 
date:   2019-05-29
thumb:  /media/fashion-iq-teaser.png
paper_name: Fashion IQ: A New Dataset towards Retrieving Images by Natural Language Feedback
conf_name: Arxiv 2019 
paper_authors: Xiaoxiao Guo*, Hui Wu*, Yupeng Gao, Steven J. Rennie and Rogério S. Feris (* equal contribution) 
paper_pdf: https://arxiv.org/abs/1905.12794
---

### Overview

Fashion IQ is a new and novel dataset we contribute to the research community to facilitate research on natural language based interactive image retrieval. High fidelity interactive image retrieval, despite decades of research and many great
strides, remains a research challenge. We believe that Fashion IQ can encourage further work on developing more natural and real-world applicable conversational shopping assistants, and serves as a new benchmark for composing natural language and image for image retrieval. In 2019, we provided Fashion IQ Challenge at ICCV 2019 workshop on [Linguistics Meets Image and Video Retrieval](https://sites.google.com/view/lingir/fashion-iq). In 2020, we will host a second challenge at CVPR 2020 workshop on [Computer vision for Fashion, Art and Design](https://sites.google.com/view/cvcreative2020/fashion-iq). 

<!--more-->

The images of fashion products that comprise our Fashion IQ dataset were originally sourced from Amazon.com. Similar to [3], we selected three categories of product items from the original [Amazon Review data](http://jmcauley.ucsd.edu/data/amazon/), specifically: Dresses, Tops&Tees, and Shirts. We collected natural language based
user feedback, describing the differences between each target
product image and a single reference product image. 
As shown in our paper [1], human-written relative descriptions are associated with real-world context, including side information derived from product descriptions and customer reviews.
This unique feature of the Fashion IQ dataset allows researchers
to investigate the advantages of natural language
feedback in conjunction with such contextual information,
which is often available in practice. The following figure shows the overall 
pipeline of the dataset collection procedure. 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-collection.png" width="600">

<br/>

### Fashion IQ Challenge v1 
To boost progress on interactive image retrieval based on natural language feedback, we release Fashion IQ at ICCV 2019 workshop on [Linguistics Meets Image and Video Retrieval](https://sites.google.com/view/lingir/fashion-iq). During the challenge, the entire training and validation set and the testing queries (each query is composed of a reference image and two relative captions) are open to public. The competition period is from June to September 2019. 

For more information, please refer to the [Fashion IQ challenge](https://sites.google.com/view/lingir/fashion-iq) official page. 

<!-- ### Fashion Datasets -->

### Dataset Access and Download  
Basic statistics of the resulting Fashion IQ dataset are summarized below.
Please download the dataset <a href="https://github.com/XiaoxiaoGuo/fashion-iq">from here.</a> 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-statistics.png">
<br/>

<!-- ### Demo Video -->


### References
<p>
  [1] Xiaoxiao Guo*, Hui Wu*, Yupeng Gao, Steven J Rennie, and Rogerio S Feris. 
 "The Fashion IQ Dataset: Retrieving Images by Combining Side Information and Relative Natural Language Feedback".(* equal contribution)  <a href="https://arxiv.org/abs/1905.12794">[pdf]</a>
  <br/>
  [2] Xiaoxiao Guo*, Hui Wu*, Yu Cheng, Steven Rennie, and Rogerio Schmidt Feris. 
  "Dialog-based Interactive Image Retrieval." NeurIPS 2018.(* equal contribution) <a href="https://papers.nips.cc/paper/7348-dialog-based-interactive-image-retrieval.pdf">[pdf]</a>
  <br/>
  [3] Z. Al-Halah, R. Stiefelhagen, and K. Grauman. "Fashion forward: Forecasting visual style in fashion". ICCV, 2017. 
</p>

