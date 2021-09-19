# Deep-Q-Network-Lunar-lander
In this project, I have implemented a DQN agent and demonstrated how to use it to solve an OpenAI Gym environment.
Here, you can see how I have used the concept of experienced replay and fixed Q-target to stabalize the neural networks.

For the Lunarlander environment details refer to the following link:

Landing pad is always at coordinates (0,0). Coordinates are the first two numbers in state vector. Reward for moving from the top of the screen to landing pad and zero speed is about 100..140 points. If lander moves away from landing pad it loses reward back. Episode finishes if the lander crashes or comes to rest, receiving additional -100 or +100 points. Each leg ground contact is +10. Firing main engine is -0.3 points each frame. Solved is 200 points. Landing outside landing pad is possible. Fuel is infinite, so an agent can learn to fly and then land on its first attempt. Four discrete actions available: do nothing, fire left orientation engine, fire main engine, fire right orientation engine.

GITHUB implementation of the environment:
https://github.com/openai/gym/blob/master/gym/envs/box2d/lunar_lander.py

Environment description:
https://gym.openai.com/envs/LunarLander-v2/
