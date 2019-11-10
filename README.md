# Project Navigation

## 1. Introduction

The goal of this project is to solve the Banana Environment. In fact it means you have to collect as many yellow bananas as you can while you have to avoid to collect blue ones.

This short animation below shows how it goes in practice.

![Trained Agent](https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif)

[source](https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation)

## 2. Some details

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

## 3. My solution

You cen find a report about my solution in details in the `Report.html` file.

If you want to run my solution on your machine or at any place in that cloudy world `Navigation.ipynb` is the file you're searching for.

If you want to jump right into the origins of the project `Navigation_Original.ipynb` is definitely your best friend now.

### 3.1. Requirements

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

### 3.2. Try the solution

If you want to test my solution you can run anything but part `3.7`.

### 3.3. Play around

If you want to see how parameters change the learning process you're welcome to play with the numbers in section `3.2`.

## 4. Improvement ideas

There are several ways to imporve the performance of an Agent with the Banana Environment. I'll plan to implement all of them.

### 4.1. Prioritized Experience Replay

Implementing Prioritized Experience Replay seems to be a good idea in the near future since it helps to improve the performance and significantly reduces the training time. I'll try it out.

### 4.2. Rainbow

As the name might suggest, Rainbow is a mixed kind of network. It is actually a DQN based off-policy deep reinforcement learning algorithm with several improvements. Currently, it is the state-of-the-art algorithm mostly used on ATARI games but it definitely worths a try.

### 4.3. Visual approach

The source repository itself cntains a notebook with the beginning code of implementing a visual approach for this problem. I'm sure it also worths a try since visual approaches are more robust ways if we think about it from a more general perspective.

