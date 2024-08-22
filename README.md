# 300Days__GenerativeAI
This repository, 300Days_GenerativeAI, is dedicated to 300 days of continuous learning focused on generative AI, studying different books and research papers daily. I'll revisit past learnings, update my understanding, and dive deeper into generative AI's intricacies.


| Book | Status |
|------|--------|
| [Mastering PyTorch: Create and deploy deep learning models from CNNs to multimodal models, LLMs, and beyond](https://www.amazon.com/Mastering-PyTorch-powerful-learning-architectures-dp-1801074305/dp/1801074305/ref=dp_ob_title_bk) (Ashish Ranjan Jha) | 🔄 Ongoing |
| [Transfer Learning for Natural Language Processing](https://www.amazon.com/Transfer-Learning-Natural-Language-Processing/dp/1617297267) (Paul Azunre) |      |    |
| [Build a Large Language Model (From Scratch) (MEAP)](https://www.amazon.com/Build-Large-Language-Model-Scratch/dp/1633437167/ref=sr_1_1?s=books&sr=1-1) (Sebastian Raschka) |      |    |
| [Learn Generative AI with PyTorch](https://www.amazon.com/Learn-Generative-PyTorch-Mark-Liu/dp/1633436462/ref=sr_1_1?s=books&sr=1-1) (Mark Liu) |      |    |
| [Generative AI in Action (MEAP V02)](https://www.amazon.com/Generative-AI-Action-MEAP-V02/dp/B08F5FX8M7) (Amit Bahree) |      |    |
| [Understanding Langchain: A Comprehensive Guide to Crafting Futuristic Language Model Applications](https://www.amazon.com/Understanding-Langchain-Comprehensive-Futuristic-Applications-ebook/dp/B0CLRPF596/ref=sr_1_1?s=books&sr=1-1) (Jeffery Owens) |      |    |
| [The Developer’s Playbook for Large Language Model Security](https://www.amazon.com/Developers-Playbook-Large-Language-Security/dp/109816220X) (Steve Wilson) |      |    |

<br>

| No. | Research Paper | Topic                        | Status    |
|-----|----------------|------------------------------|-----------|
| 1   | [Going Deeper with Convolutions](https://arxiv.org/pdf/1409.4842) | GoogLeNet | ✅ Completed |


### Day 1 of 300DaysOfGenerativeAI
- In today's session on Mastering PyTorch, I focused on the foundational aspects of deep learning, particularly through the "Deep Learning with PyTorch: A 60 Minute Blitz" tutorial. I learned about neural network architectures, including fully connected, convolutional, and recurrent layers, and explored PyTorch's key modules such as torch.autograd for automatic differentiation and torch.nn for building networks. I practiced forward and backward propagation, loss calculation, and gradient descent, culminating in the construction of a simple feed-forward neural network. On upcoming sessions, my agenda includes a deep dive into the power of Convolutional Neural Networks (CNNs), their architectural evolution, and hands-on development of models like LeNet, AlexNet, VGG, GoogLeNet, Inception v3, ResNet, DenseNet, and EfficientNets, discussing their significance and future in deep learning.
- Additional Resource:
  - [Deep Learning with PyTorch: A 60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html)

### Day 2 of 300DaysOfGenerativeAI
- In today's session on Mastering PyTorch, I have a brief but productive session diving into deep CNN architectures. I explored why CNNs are so effective for tasks like image classification and object detection, highlighting their parameter efficiency, automatic feature extraction, and hierarchical learning. I reviewed various architectural innovations such as spatial, depth, width, and multi-path-based CNNs. I also examined an implementation of AlexNet in PyTorch, focusing on its layer structure and how it leverages dropout and activation functions. Additionally, I noted the availability of various pre-defined CNN models in PyTorch’s torchvision package, including AlexNet, VGG, ResNet, and others.

### Day 3 of 300DaysOfGenerativeAI
- In today's session on Mastering PyTorch, I have prepared a dataset for an image classification task, implemented a fine-tuning process for a pre-trained AlexNet model, and addressed a deterministic behavior issue that arose during training. I created data loaders, defined helper functions for visualization and model fine-tuning, and modified the final layer of the pre-trained model to match the number of classes in my dataset. During the fine-tuning process, I encountered a warning related to the use of the `adaptive_avg_pool2d_backward_cuda` operation, which does not have a deterministic implementation. To address this, I learned about different approaches to enable deterministic behavior in PyTorch, such as selectively disabling determinism for the problematic operation or using the `warn_only=True` option when enabling deterministic algorithms.This hands-on experience has provided me with a deeper understanding of practical considerations when applying deep learning techniques to image classification problems.

### Day 4 of 300DaysOfGenerativeAI
- In today's session on Mastering PyTorch, I have learned that GoogLeNet, also known as Inception v1, is a groundbreaking convolutional neural network architecture that introduced the inception module, which features parallel convolutional layers with varying kernel sizes (1x1, 3x3, 5x5) to capture multi-scale features. I have discovered that 1x1 convolutions are crucial for dimensionality reduction, allowing the model to maintain efficiency by reducing the depth of feature maps without altering spatial dimensions. Additionally, I have learned that GoogLeNet employs global average pooling before the output layer to minimize parameters and enhance robustness against overfitting. My exploration of Inception v3 has shown me how it builds upon the original design with more complex modules and additional layers, resulting in improved performance. Overall, I now have a deeper understanding of the innovative techniques in GoogLeNet and Inception v3, including inception modules, 1x1 convolutions, and global average pooling, which have significantly advanced the field of computer vision.

### Day 5 of 300DaysOfGenerativeAI
- In today's session on Mastering PyTorch, I worked on implementing the GoogLeNet architecture, focusing on the construction and integration of multiple Inception modules within the network. I refined the parameters of each Inception module to correctly reflect the intended configuration, which included adjusting the convolutional and pooling layers to efficiently extract features at various scales. Additionally, I incorporated the initial convolutional layer with batch normalization and ReLU activation, followed by max pooling layers for downsampling. While working on the model, I also considered the importance of auxiliary classifiers, which are typically included in the GoogLeNet architecture to help mitigate the vanishing gradient problem by providing intermediate supervision. These classifiers are smaller versions of the main classifier, attached to earlier layers, and they improve the network's ability to learn meaningful features during training.


