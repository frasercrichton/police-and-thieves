# dalle-mini

![cop](https://user-images.githubusercontent.com/52700324/175556508-9ea39768-7ad1-4d96-a93e-3eef5d3e7386.png)

Try Dalle Mini here:

[https://huggingface.co/spaces/dalle-mini/dalle-mini](https://huggingface.co/spaces/dalle-mini/dalle-mini)

# Running the Jupyter Notebook

## Prerequisites 

* a [Google Account](https://support.google.com/accounts/answer/)
* a [Weights & Biases account](https://wandb.ai/site)

## Running Jupyter Notebooks in Google Collab 

[Learning the CoLab Jupyter Notebook Environment](https://www.webagesolutions.com/blog/learning-the-colab-jupyter-notebook-environment)




The limitations of the model and its Misuse, Malicious Use, and Out-of-Scope Use 

https://huggingface.co/dalle-mini/dalle-mini


he model has only been trained with English descriptions and will not perform as well in other language

Content that is potentially problematic should be filtered out, e.g., via automated models that detect violence or pornography.
Further work on this model should include methods for balanced and just representations of people and cultures, for example, by curating the training dataset to be both diverse and inclusive.


* [Conceptual Captions Dataset](https://aclanthology.org/P18-1238/), which contains 3 million image and caption pairs.

https://github.com/google-research-datasets/conceptual-captions


* [Conceptual 12M](https://arxiv.org/abs/2102.08981), which contains 12 million image and caption pairs.
https://github.com/google-research-datasets/conceptual-12m

The OpenAI subset of YFCC100M, which contains about 15 million images and that we further sub-sampled to 2 million images due to limitations in storage space. They used both title and description as caption and removed html tags, new lines and extra spaces.

For fine-tuning the image encoder, a subset of 2 million images were used. All images (about 15 million) were used for training the Seq2Seq model.
