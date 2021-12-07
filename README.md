# AIPI 530 Final Project - Ningyi Xue


This repo is for AIPI 530 final project, and the goal of this project is to build a pipeline for offline reinforcement learning on top of [d3rlpy](https://github.com/takuseno/d3rlpy)

## Preface - Reinforcement Learning
Please check out this [blog](https://ningyixue.medium.com/basic-introduction-of-reinforcement-learning-65a48e305a9d) post for basic understanding of reinforcement learning. The following information is included in the blog post:
- What is reinforcement learning?
- What are the pros and cons of reinforcement learning?
- When should we consider applying reinforcement learning (and when should not)?
- What's the difference between supervised learning and reinforcement learning?
- What is offline reinforcement learning?
- What are the pros and cons of offline reinforcement learning?
- When should we consider applying offline reinforcement learning (and when should not)?
- An example of offline reinforcement learning in the real-world.


## Installation
### Please follow the below steps for installation:
### Step 1:
Git clone this repository:
- !git clone https://github.com/ningyixue/AIPI530_Final_Project.git
### Step 2:
Install packages if you don't have:
- !pip install Cython numpy
- !pip install -e
### Step 3:
Install pybullet:
- !pip install git+https://github.com/takuseno/d4rl-pybullet

## Execution
- !python train_cql.py

#### Please note: my default setting for epochs is 20, and you can make changes if you go cql_train.py, and change the number after "EPOCHS:". 

My Colab example: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1lrWwum2tzp38XVESQ-OC0GLQYbQSwRaV#scrollTo=Wcpp9bHNJD1l)

## Logs and Plot in the Above Colab Example
#### There are three logs that are saved and used for plotting purposes:
- environment_cql.csv (CQL - For average reward)
- estimated_q.csv (CQL - For estimated q value)
- init_value.csv (FQE - For FQE estimated q value)

#### You can find the three files under '/d3rlpy/examples/pybullet/d3rlpy_logs' once you finished running cql_train.py

Here is the graphs received from the most recent execution with 20 epochs:
![img.png](https://github.com/ningyixue/AIPI530_Final_Project/blob/main/offline_rl.png)



## citation
The repository is modified on top of [d3rlpy](https://github.com/takuseno/d3rlpy).
