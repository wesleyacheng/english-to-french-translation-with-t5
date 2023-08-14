# english-to-french-translation-with-t5
English to French Translation with T5

# Introduction

Hello, I'm Wesley, nice to meet you! 👋

There are in general two types of deep learning models - **discriminative** and **generative** models. 

An example of a **discriminative** model in NLP is a **text classification model** like my previous notebook *[Twitter Emotion Classification with BERT](https://www.kaggle.com/code/wesleyacheng/twitter-emotion-classification-with-bert)* where we classified each tweet into one of three emotions - joy, anger, and sadness.
On the other hand, an example of a **generative** model in NLP is an **autoregressive text model** like the recently mainstream **ChatGPT** where it predicts/generates its next words based on the input sentence you provide it with.

Here's an example of what a **generative** NLP model can do.

<img width="51" alt="Screenshot 2023-08-12 at 4 40 49 PM" src="https://github.com/wesleyacheng/english-to-french-translation-with-t5/assets/15952538/cb81bfb0-fec0-46a7-8350-309bb7101294">

![Screenshot 2023-08-12 at 4 43 32 PM](https://github.com/wesleyacheng/english-to-french-translation-with-t5/assets/15952538/3abf07b5-7a14-45e3-ae73-a8a14e12b0a5)


Here's the link to their [blog post](https://openai.com/blog/chatgpt) if you want to know more about **ChatGPT** and how it was fine-tuned from GPT-3.5 with reinforcement learning.

The **main difference** between a **discriminative** model and a **generative** model is that **discriminative** models *predict where a new unknown data point might fit in its data distribution based the dataset it was trained on*, hence it outputs a class/category; while a **generative** model *uses the new unknown data point as a starting point to predict/generate new data points that are highly related to it*, hence it outputs similar content that is highly related to the input it was given.
 
These two types of models are different as they tackle different problems. **Discriminative** models tackle the problem of *how to split the dataset into clusters with similar features*, while **generative** models tackle the *problem of how to use the dataset to make new data that are highly similar to it*.

![Screenshot 2023-08-13 at 10 22 32 PM](https://github.com/wesleyacheng/english-to-french-translation-with-t5/assets/15952538/0fc54f94-09a4-41d8-8a02-d600336b6291)

As an introduction to **generative** models in **Natural Language Processing (NLP)** in this notebook, we will be doing the **classic machine translation task** (a **generative** problem) of translating **English to French** by transfer learning with **Google's T5 model** [\[blog\]](https://ai.googleblog.com/2020/02/exploring-transfer-learning-with-t5.html). We will be using the *HuggingFace NLP interface* to simplify this introduction. Let's get going! 🦾
