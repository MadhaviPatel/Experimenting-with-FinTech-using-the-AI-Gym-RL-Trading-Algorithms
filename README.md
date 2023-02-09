# Experimenting-with-FinTech-using-the-AI-Gym-RL-Trading-Algorithms


Action :
- Step 1 
Collected data from Microsoft

- Step 2 
Gym environment create by using reference given by professor
First we will implementing _init__ function of our environment class, The observation and action spaces will be defined.
     -   Observation Space 
The observation space can be discrete or continuous. .It is defined by cells, and the agent could be inside one of those cells, which contains all of the data in the environment that the agent would then observe.
     -   Action Space 
In addition, the action space can be either continuous or discrete. We define the type and shape of our action space in the constructor, which will contain all of the actions which an agent could really take in the environment.
After that we will define functions in Env class

- Step 3
Applying an action to a step in the environment executes it. The new observation, reward, completion status, and other information are returned.
 
- Reset 
Returns the initial observation after resetting the environment to its initial state.
 
- Render 
The render method can be used to print a rendition of the environment on a regular basis. It could be as straightforward as a print statement.
-  _next_observation 
The _next observation method gathers stock data from the previous five days, adds the agent's account information, and scales all values to between 0 and 1.
 
- _take_action 
The take action method must execute the model's action and either buy, sell, or hold the stock.
 We can now use a data frame to create a StockTradingEnv environment and test it with a model from stable-baselines.
 
 
Now, using an agent that performs random actions, perform some actions in the environment.
