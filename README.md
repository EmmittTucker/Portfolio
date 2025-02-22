# Emmitt J Tucker's Coding Portfolio
Last updated: 2/22/2025
## About Me
My name is Emmitt J Tucker. Currently I am a master's student enrolled in Northeastern's MS Align program as part of the Fall 2024 cohort. Prior to enrolling at Northeastern, I completed my B.S. in Biology from the University of Massachusetts Boston in 2018 before working in the Biotech industry for 5 years. I was also attempted to start my own gaming company named Absurd-i-Oh that would attempt to make citizen science more popular. Throughout my time in Biotech, I focused heavily on lab automation through both lab robotics and automation coding. I have a wide variety of topics I am interested ranging from Human-AI collaboration to evolutionary computation. I plan to pursue a PhD program upon completion of my M.S. degree. 
<br><br>
Outside of programming I enjoy gaming and movie culture (particularly horror movies). My interest in gaming in particular has greatly influenced my personal projects as I assume you will see through my projects.  
<br><br>
If you would like to connect, please reach out on LinkedIn and mention that you found me through this portfolio (Link: https://www.linkedin.com/in/emmitt-tucker-45ba52159/).
## Current Projects
This section covers the current projects I work on in my free-time.<br>
### Project Aquarium
This is a project inspired by my background in biology and interest in **natural selection** and **selective pressure**. The focus of this work is **simulated experimental evolution**. This project contains a simulation that uses cooperative NeuroEvolution to produce classificatication artificial neural network candiates for further investigation. In the simulation, neural network systems are represented as individual "fish" that move around their environment. The goal of this project is to both visualize and automate neural network optimization. 
<br><br>
This project was heavily assisted with the help of prompt engineering using **OpenAI's chatGPT-o3-mini model**. This model did a decent job with handling requests, although it would sometimes give me answers to previous questions when prompted. One consistent error I found was that it would have to be reminded of how changes it made effected the rest of the code base. the o3-mini model was also somewhat helpful when it came to understanding how neural networks worked. It was not helpfull when it came to trying to figure out different evolution mechanics that would lead to better results. This may have been the result of me telling the o3-mini model to specialize as an AI specialist at the start of the conversation. 
<br><br>
The systems of the fish are made of 5 different neural networks that control the behavior and survival chances.Their movement is controlled by the **Behavior Net** (B-Net). This network learns over time and adapts movement if the individual is not finding resources. Individuals are spawned with no movement memory, and they learn better patterns throughout their lifetime (ideally). The behavior network processes a scalar value depending on what **mode** this fish is in which determines what actions it does in the environment. The output of the network is interpreted as an angular change in the fishes direction. 
<br><br>
The fish also have a **classification network**, which is the primary subject of interest for this project. The goal of the classification network is to work with a <ins> binary classification</ins> task and make the correct prediction. This project was designed around the open-source Wisconson breast cancer dataset (link: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data/data). The final working version of this project should be able to work with any dataset that can be used for binary classifcation (including datasets with numerical and caterogical data). The classification networks have input nodes dependent on the features of the provided dataset. The classifcation network has several other "helper" networks that determine the composition of the classification network. These networks are currently named **Managers** in the code base. First, there is the feature manager. The feature manager filters the dataset that gets provided to the classification network. Next there are hyperparameter and architecture managers as well. These networks work together to change the composition of the classification network. These managers learns from interactions with resources to learn the importance of different composition features dependent on the dataset provided. 
<br><br>
Their objective is to survive by collecting resources that represent elements from the chosen dataset. Resources appear in random locations throughout the area portion of the screen. When a resource gets within the detection range of a fish, the fish will head towards that resource. Currently, resources can represent between 1 and 5 elements from the dataset. The frequency in the resources appear correlates with the number of elements that resource represents (1 appears more than 5). When the fish is in **feeding** mode and comes into contact with the boarder of the resource, it attempts to feed on it by classifying the elements of that resource. If the classification is successful, the fish gains energy from that resource. Fish compete for resources through combat when another fish comes within range of their combat zone while they are pursing a resource. Individuals that die will drop the resources that they have consumed. Once fish have consumed a sufficient number of resources (5), they will "mature" and pursue mating with another fish that is also in **mating** mode. The accuracy of the fish's classification of different resources in the environment determines their size, detection range, combat power and mating prowess. If an individual is not in feeding or mating mode, they wander around the arena at random in **wandering** mode. 
<br><br>
When the fish mate, their genomes are subject to both cross over and mutation. Fish are always spawned with no accuracy score and in feeding mode. The number of fish reproduced is determined by the default cost to reproduce. It is also possible for the default parameters of the initial population to change throughout reproduction. Fish have a **tier** determined by their accuracy which influences mating behavior. There are 3 tiers that change according to the fish's current accuracy score. A difference in tier reducing a successful mating attempt by 25%. The fish have a memory of who they have competed for food with and they will not mate with those they have fought. 
<br><br>
My idea was that selective pressure applied to the neural networks through competition and their environment would lead to success neuroevolution. 
<br><br>
The look of the fish is inspired by the features of their different networks. The head is the only part of the all creatures which is consistent. 
<br><br>
#### Observations
From my experiments so far, I have observed several consistent events with the current settings. 
#### Future Work

## Previous Projects

### Neural Network War

### Abusrd-i-Oh!

### Woman's Advancement Neural Network

