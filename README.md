# Police and Thieves

![cop](https://user-images.githubusercontent.com/52700324/175556508-9ea39768-7ad1-4d96-a93e-3eef5d3e7386.png)
![23](https://user-images.githubusercontent.com/52700324/175558040-adac32a0-b429-4d7e-ae59-c08e15213d7a.jpg)
![27](https://user-images.githubusercontent.com/52700324/175558076-f28580f9-3827-4a99-88cb-1f4c785b6007.jpg)


Craiyon (the rebranded name of DALL·E mini) is an AI model that creates computer-generated images from text prompts. It uses a model trained using captioned images from datasets available on the internet. Here, it's been given the text prompt 'cop' to generate the image above.

Police violence, corruption and the way in which police fail victims of crime have all become key issues in how we have come to understand police in recent years. Craiyon provides a seemingly ambiguous way of considering who police are and what role they have in society. None of the images Craiyon returns are real and yet real images contribute to Craiyon's 'sense' of what a police officer is.

The bias that is inherent in every aspect of computer vision is a useful tool. It allows us to deconstruct the institutions that create these technologies and it also allows us to see something of police as an institution itself. Of 99 images returned for the term 'cop' - all were white (only one could be identified as possibly African American) and none were identifiable as a woman. Does this bias come from the technologist's model or dataset? Does it come from the way police are visually represented in society? Or does it come from the bias inherent in institutions like the police?

At this time in generative computer vision, it's still possible to see the traces of the original images in the generated images and identify some of the incidents that are present in the datasets that power machine learning's models.

I'd like to investigate a little more about this as a topic so I'm going to do that as an Instagram project sharing more as I learn here.

Try Craiyon here:

[https://www.craiyon.com/](https://www.craiyon.com/)

Limited to 6 images of 256x256 at at time.

# Generating more images

To get round the limit of six I'm running the Jupyter Notebook included here. It's based on original work here [SOLVED - DALL-E Mini: Too much traffic, please try again by Dave Davies](https://wandb.ai/onlineinference/ml-news/reports/Beating-The-DALL-E-Mini-Too-much-traffic-please-try-again---VmlldzoyMTg4Mjkz)


# Running the Jupyter Notebook

The Jupyter Notebook included here allows to generate more images and save them to Google Drive. It also allows for customising other aspect of the image generation,

## Prerequisites 

* a [Google Account](https://support.google.com/accounts/answer/)
* a [Weights & Biases account](https://wandb.ai/site)

## Running Jupyter Notebooks in Google Collab 

[Learning the CoLab Jupyter Notebook Environment](https://www.webagesolutions.com/blog/learning-the-colab-jupyter-notebook-environment)


## Datasets

* [Conceptual Captions Dataset](https://aclanthology.org/P18-1238/), https://github.com/google-research-datasets/conceptual-captions which contains 3 million image and caption pairs.

* [Conceptual 12M](https://arxiv.org/abs/2102.08981), which contains 12 million image and caption pairs.
https://github.com/google-research-datasets/conceptual-12m

* The OpenAI subset of YFCC100M, which contains about 15 million images and that we further sub-sampled to 2 million images due to limitations in storage space. They used both title and description as caption and removed html tags, new lines and extra spaces.

For fine-tuning the image encoder, a subset of 2 million images were used. All images (about 15 million) were used for training the Seq2Seq model.



Running on SageMaker

Lifecycle script
https://gist.github.com/ottok92/ed6d6b8ec5526b1ec52980812c52da96