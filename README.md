# Reinforcement Learning :computer:


The objective of this task was to train an agent to decently play the Atari game Breakout within a Gymnasium environment. 

This task was an assignment as part of my Masters in Data Science course with the University of Malta. 

### Introductory Notes

Hardware and operating system architecture used for the assignment:
-	OS : Ubuntu 22.04
-	RAM : 64Gb
-	GPU : NVIDIA Corporation GA104 [GeForce RTX 3060 Ti Lite Hash Rate]
-	Processor : 1th Gen Intel® Core™ i7-11700F @ 2.50GHz × 16
-	Gymnasium version : 0.29.1

### General

The training of the model was performed over 50,000 episodes, where each episode is taken as a full game of 5 lives. The total training time on the indicated hardware was of circa 5 hours. The model weights of the trained model are saved for convenience and immediate upload. The algorithm is set such that if a pre-trained model is found, the pre-trained weights are loaded. If not, a new training session is initiated. 

Please note that while I have tried to maintain reproducibility as much as possible (by initializing the weights of a new model using a generator), the stochastic nature of the model cannot guarantee the same levels of performance as the saved model.  

### Architecture

The following architecture was used for the neural network. 

![final_architecture drawio](https://github.com/user-attachments/assets/747aa5dc-1fba-480e-a23a-68ba431461be)

### Evaluation

Below is a visualization (using Tensorboard) of the loss over the training epochs:

![loss_train](https://github.com/user-attachments/assets/f1268fc2-f5dd-4c27-ad8b-a4d1896f5a28)

And below is a visualizaton (using Tensorboard) of the score for each game over the training epochs:

![score_train](https://github.com/user-attachments/assets/24de742c-5b34-47ff-b985-745e7aa933a3)


### Trained Agent

The following gif is the result of the trained agent playing Breakout. 

![breakout](https://github.com/user-attachments/assets/425eef28-75d2-4411-9bfe-a52aad359d10)

