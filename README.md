# Current-Emerging-Trends-in-CS
CS-370


In this project, I analyzed and refined existing Python code, implementing a Q-learning algorithm for a maze-solving task. The code forms part of a reinforcement learning setup where an agent learns to navigate through a maze to find a treasure.

# Code Provided:
Maze Environment (TreasureMaze class): This class represents the maze as a two-dimensional Numpy array. It includes functionality for resetting the agent's position, updating its state based on actions, and tracking rewards.

Agent's Experience Storage (GameExperience class): This class is designed to store the agent's experiences (or episodes), which include the states, actions, and rewards during each attempt to solve the maze.

Neural Network Model for Decision Making: A part of the setup involved defining a neural network model using Keras, which the agent uses to make decisions based on its current state.

Some of the Training Function (qtrain): The main function provided for training the agent using deep Q-learning. It includes the logic for running episodes, updating the agent's state, and adjusting the balance between exploration and exploitation.

# What code did you create yourself?
I complete the Q-learning training algorithm in the qtrain function by implementing a loop over epochs as outlined in the pseudocode. This loop will involve the agent navigating through the maze, updating its state based on actions taken, and training the neural network model on the experiences gained. 

Error Handling for Invalid Actions: A check to ensure that the agent has valid actions to choose from. If not, we can break the episode loop and consider it a loss.

Validation for Input Parameters: Add checks at the start of the qtrain function to validate the maze structure and the neural network model.

Epoch Loop: The loop iterates over the specified number of epochs.

Agent Initialization: Each epoch starts by placing the agent in a random free cell.

Episode Loop: The agent navigates the maze until it either wins or loses.

Action Selection: The agent selects actions based on either exploration (random choice) or exploitation (using the model's predictions).

Experience Storage: The agent's experiences (state, action, reward, new state, and game status) are stored.

Model Training: The model is trained on a subset of the agent's experiences.

Tracking and Printing Info: The loop keeps track of various metrics like win rate and prints them out for each epoch.

Termination Check: The loop checks whether the agent has achieved a consistent win rate and if it can complete the maze from all positions. If these conditions are met, the training ends.


# What Do Computer Scientists Do and Why Does It Matter?
Problem Solving: Computer scientists address complex problems by developing algorithms and creating efficient software solutions. This problem-solving skill is crucial in various fields, including healthcare, finance, and technology, impacting how these industries operate and evolve.

Innovation and Technology Development: They are at the forefront of technological advancements, designing new software, improving computer hardware, and developing new ways to use technology. Their work in areas like artificial intelligence, data science, and cybersecurity significantly shapes our digital landscape.

Data Analysis and Management: With the increasing importance of big data, computer scientists analyze and interpret large sets of data to help organizations make informed decisions. This role is essential for driving growth, optimizing operations, and understanding trends.

Research and Education: Many computer scientists engage in research, contributing to the academic and scientific community. They also educate the next generation of tech professionals, sharing knowledge and skills that are critical for future innovations.

# Approaching a Problem as a Computer Scientist
Define the Problem: Clearly understand what the problem is and what the desired outcome looks like.

Research and Analysis: Gather relevant information and analyze existing solutions or similar problems.

Design Algorithms: Develop algorithms that provide a step-by-step solution to the problem.

Implement Solutions: Code the algorithms into a software solution, using appropriate programming languages and tools.

Testing and Iteration: Test the solution rigorously and iterate based on feedback and testing results.

Evaluation and Deployment: Evaluate the effectiveness of the solution in a real-world environment and deploy it for use.

# Ethical Responsibilities
To End Users: Respect privacy and data security, ensure accessibility, and create user-friendly designs. Avoid harm and ensure the technology benefits users without causing unintended negative consequences.

To the Organization: Maintain professional integrity, protect confidential information, and work towards the organization's goals without compromising ethical standards.

To Society: Consider the broader impacts of technology on society, including potential job displacement, societal changes, and ethical use of AI and data.

Continual Learning: Stay updated with ethical standards, legal requirements, and technological advancements to ensure responsible practice.
