# DeepRace-Model 🚙
![IncentiveBasedGoalsDark 3cc13d53](https://user-images.githubusercontent.com/95357174/197383453-19b54181-819e-4b9d-addf-bbd72966ed9e.svg)

Steps Involved : 
 1. Name your Model
 2. Choose Track
 3. Choose Algorithm type
 4. Customize reward function
 5. Choose duration


 # Before we started

In this we will train a reinforcement learning (RL) model and see a simulation of how that model performs on a track. The AWS DeepRacer Student League is where you compete for the fastest lap times with you friends. You have the option to opt out of submitting your trained model to the Student League.

 # How is an RL model trained?

In AWS DeepRacer, an agent (car) learns from an environment (track) by interacting with it. During training, the model iterates and updates different parameters based on rewards received.

 # Model training is an iterative process :_

Training a model is like creating a prototype. Each model iteration is a step towards finding the optimal parameters. When training has finished, clone your model to continue improving it.

  # Improving your model 

After training an initial model, you can use the current state of the model's parameters as the starting point for the next model by choosing clone model. Submit to the leaderboard to evaluate your model's performance. Look for the race time and the number of times your car went off track.

#  To get started
give your model a unique name. This will help you find your model later when you want to clone and improve it. Be specific and descriptive. You cannot change the name of your model after training has begun.

Model name:-

 🏁Required
The model name can have up to 64 characters. Valid characters are a-z, A-Z, 0-9, and - (hyphen). No spaces or underscores.

# How to choose a track ⤵️
The track you select is the environment that the agent (your car) interacts with during model training. For more challenging tracks, more training time and a more complex reward function may be required. Start simple and work your way up.

![image](https://user-images.githubusercontent.com/95357174/197383841-bcdebc85-1722-4702-9ccc-5a97acce68ef.png)
![image](https://user-images.githubusercontent.com/95357174/197383859-daa3b4e5-2568-4c1e-813e-868311c8c13e.png)
![image](https://user-images.githubusercontent.com/95357174/197383865-8140972d-726f-4b60-9f27-f9e594586b45.png)
![image](https://user-images.githubusercontent.com/95357174/197383876-685de6b9-e709-4c4e-8d1f-343c6fb9535e.png)
![image](https://user-images.githubusercontent.com/95357174/197383887-4bf55f5a-d650-41a6-bd6f-e0a74858a60c.png)
![image](https://user-images.githubusercontent.com/95357174/197383896-5bca90ce-a3eb-4330-80bb-ed93cc8ab5fe.png)
![image](https://user-images.githubusercontent.com/95357174/197383898-e9616f49-109e-4527-b881-5047d44779b8.png)
![image](https://user-images.githubusercontent.com/95357174/197383902-084c03e2-0fb1-4fc4-b492-91acf4bb48bc.png)
![image](https://user-images.githubusercontent.com/95357174/197383906-74ef524f-73a7-4ea9-a364-43d6f0e57a12.png)
![image](https://user-images.githubusercontent.com/95357174/197383908-2537ae54-52bd-44f1-92dd-689c7b971089.png)
![image](https://user-images.githubusercontent.com/95357174/197383915-ace4b32e-8ce5-44c2-a002-e22524c89b3a.png)
![image](https://user-images.githubusercontent.com/95357174/197383921-8d969021-0758-456a-b8c5-26b3d59b37fb.png)


# Choose algorithm type
A model training algorithm is a procedure that uses data to create a model. These algorithms maximize total reward differently. Proximal Policy Optimization (PPO) explores the environment less compared to Soft Actor Critic (SAC).
## Proximal Policy Optimization (PP0)
      Needs more data to produce consistent results
## Soft Actor Critic (SAC)
     Uses less data but produces less consistent results
# Customize reward function ⤵️
 
 ## What is a reward function?
 
The reward function is Python code that describes immediate feedback in the form of a reward or penalty to move from a given position on the track to a new position.

 ## What is the purpose of a reward function?
 
The reward function encourages the vehicle to make moves along the track quickly to reach its destination.

## Choose and modify one of the sample reward functions.
     1.Follow the centerline
         Sections the track into three reward zones. The farther the car strays from the centerline, the less it’s rewarded.
     2.Stay within borders
         Defines the track border and gives high rewards if all 4 wheels stay on the track, which leaves it to the model to find the optimal path.
     3.Prevent zig-zag
          Is the centerline reward function plus a steering angle range limit. Keeps the car driving smoothly down the middle.
# Choose duration
   The duration of model training time impacts the performance of your model. It’s just like learning a skill: the longer you practice, the better you get at it.
  ## Choose duration of model training
      Training time must be between 10 and 600 mins.
      Time must be between 10 and 600 minute

You have successfully crafted a reward function and are now ready to train the model. Submit to the leaderboard to evaluate your performance.

