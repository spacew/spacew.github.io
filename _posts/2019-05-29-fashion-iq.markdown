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

The images of fashion products that comprise our Fashion IQ dataset were originally sourced from Amazon.com. Similar to [3], we selected three categories of product items from the original [Amazon Review data](http://jmcauley.ucsd.edu/data/amazon/), specifically:Dresses, Tops&Tees, and Shirts. Additionally, for each image, we crawled Amazon.com and extracted corresponding product information, when available. We collected natural language based
user feedback, describing the differences between each target
product image and a single reference product image.
Note that these human-written relative descriptions are associated
with real-world context, including side information
derived from product descriptions and customer reviews.
This unique feature of the Fashion IQ dataset allows researchers
to investigate the advantages of natural language
feedback in conjunction with such contextual information,
which is often available in practice. The following figure shows the general 
pipeline of the dataset collection procedure. 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-collection.png" width="600">

<br/>

### Fashion IQ Challenge v1 
To encourage research on image retrieval based on natural language feedback, we release Fashion IQ at ICCV 2019 workshop on [Linguistics Meets Image and Video Retrieval](https://sites.google.com/view/lingir/challenge). During the challenge, the entire training and validation set and the testing queries (composed of reference image and relative captions) are release. The competition period is from June 10th to September 30th. For more information, please refer to the [Fashion IQ challenge](https://sites.google.com/view/lingir/challenge) page. 

<!-- ### Fashion Datasets -->

### Dataset Access and Download  
Basic statistics of the resulting Fashion IQ dataset are summarized below.
Dataset <a href="https://github.com/XiaoxiaoGuo/fashion-iq">is available here.</a> 

<img alt="img" src="{{site.baseurl}}/media/fashion-iq-statistics.png">
<br/>

<!-- ### Demo Video -->



### References
<p>
  [1] Xiaoxiao Guo*, Hui Wu*, Yupeng Gao, Steven J Rennie, and Rogerio S Feris. 
 "The Fashion IQ Dataset: Retrieving Images by Combining Side Information and Relative Natural Language Feedback".(* equal contribution)  <a href="https://arxiv.org/abs/1905.12794">[pdf]</a>
  <br/>
  [2] Xiaoxiao Guo*, Hui Wu*, Yu Cheng, Steven Rennie, and Rogerio Schmidt Feris. 
  "Dialog-based Interactive Image Retrieval." NIPS 2018.(* equal contribution) <a href="https://papers.nips.cc/paper/7348-dialog-based-interactive-image-retrieval.pdf">[pdf]</a>
  <br/>
  [3] Z. Al-Halah, R. Stiefelhagen, and K. Grauman. "Fashion forward: Forecasting visual style in fashion". ICCV, 2017. 
</p>

