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
This is a project inspired by my background in biology and interest in natural selection. This project contains a simulation that uses cooperative NeuroEvolution to produce classificatication artificial neural network candiates for further investigation. In the simulation, neural network systems are represented as individual "fish" that move around their environment. The goal of this project is to both visualize and automate neural network optimization. 
<br><br>
This project was heavily assisted with the help of prompt engineering using OpenAI's chatGPT-o3-mini model. This model did a decent job with handling requests, although it would sometimes give me answers to previous questions when prompted. One consistent error I found was that it would have to be reminded of how changes it made effected the rest of the code base. the o3-mini model was also somewhat helpful when it came to understanding how neural networks worked. It was not helpfull when it came to trying to figure out different evolution mechanics that would lead to better results. This may have been the result of me telling the o3-mini model to specialize as an AI specialist at the start of the conversation. 
<br><br>
The systems of the fish are made of 5 different neural networks that control the behavior and survival chances.Their movement is controlled by the Behavior Net (B-Net). This network learns over time and adapts movement if the individual is not finding resources. Individuals are spawned with no movement memory, and they learn better patterns throughout their lifetime (ideally). The behavior network processes a scalar value depending on what "mode" this fish is in which determines what actions it does in the environment. The output of the network is interpreted as an angular change in the fishes direction. 
<br><br>
The fish also have a classification network, which is the primary subject of interest for this project. The goal of the classification network is to work with a binary classification task and make the correct prediction. This project was designed around the open-source Wisconson breast cancer dataset (link: https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data/data). The final working version of this project should be able to work with any dataset that can be used for binary classifcation (including datasets with numerical and caterogical data). 
<br><br>
The classifcation network has several other "helper" networks that determine the composition of the classification network. These networks are currently named "Managers" in the code base. 
<br><br>
Their objective is to survive by collecting resources that represent elements from the chosen dataset. 
<br><br>
## Previous Projects

### Neural Network War

### Abusrd-i-Oh!

### Woman's Advancement Neural Network

