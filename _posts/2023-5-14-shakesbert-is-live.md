---
title: "ShakesBERT is now live!"
date: 2023-05-14T22:45:30-04:00
categories:
  - blog
tags:
  - Machine Learning 
  - My Own Projects
link: http://shakesbert.com
---

ShakesBERT was our final project for the class Machine Learning: Deep Learning. In our project, we tried to finetune a BERT model in general poetry dataset then in Shakespeare poetry dataset to do masked task. Originally, we wanted to build a multimodal BERT model with both semantic embeddings and phonetic embeddings (meters), but we failed to find a pre-trained BERT model that has these two embeddings available on the internet and thus we had to use a normal BERT. A phonetic embedding with information about how the words sound would make sense since this is a big component in word choice in poems. But we just had to make do with a normal BERT("bert-base-uncased") given the time and resources we have (which is not enough to train a transformer model all over again).

We had solid results and even got the Intuitive Surgical Best Project Award (we had an award for best final project in the deep learning class, and we got the best project award - 2 out of 30+ groups. Yay!). We only had a little mock website using ngrok to tunnel all requests to my laptop (when it's open of course) during presentation, but I decided to continue and migrated the whole thing to the website at shakesbert.com (deployed on DigitalOcean using the 200-dollar-free-credits). I learned a lot in the process and have grown to a qualified web developer (just kidding). The usage of this website is quite limited as all learning projects are (and quite ugly, my bad). Nonetheless, I am quite proud of it as it's my first non-static website (yes my first website is this static blog). Come check out [**my website (shakesbert.com)**](http://shakesbert.com)! 


Note: it can be quite slow (not because the model is slow) since I am on a tight budget for the servers.