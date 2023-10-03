# Reinforcment-Learning-Maintenance
Reinforcement Learning Based Maintenance Decision Making for Deteriorating Systems
## Overview
This essay, titled "Remaining useful life (RUL) based maintenance decision making for deteriorating systems" by Phuc Do Van, Eric Levrat, Alexandre Voisin, and Benoit Iung, aims to minimize the cost of repairing a deteriorating machine. The essay adopts a proactive condition-based maintenance (CBM) approach that uses RUL prognosis to select the optimal maintenance action. conversly,we employ a Q-learning algorithm to train an agent to find the best policy for repairing the system. The essay defines T as the time of inspection and q as the confidence interval of estimation. we try to find the optimal T for each q and by the end, the have been compared.


## what is the problem

The environment of the deteriorating system that is used in the essay "Remaining useful life (RUL) based maintenance decision making for deteriorating systems" by Phuc Do Van, Eric Levrat, Alexandre Voisin, and Benoit Iung is a hypothetical scenario that simulates a system that degrades over time and can be maintained by either perfect or imperfect actions. The system is assumed to follow a nonlinear Wiener process, which is a stochastic degradation model that captures the randomness and uncertainty of the degradation process. The system is inspected periodically, and the degradation level is measured by a sensor. The system fails when the degradation level exceeds a predefined threshold. The perfect maintenance action restores the system to the "as good as new" state, while the imperfect maintenance action restores the system partially, depending on the allocated maintenance cost, the system age, and the number of previous imperfect maintenance actions. The essay proposes an adaptive maintenance policy that uses the RUL prognosis to select the optimal maintenance action at each inspection time. The RUL prognosis is based on estimating the parameters of the degradation model using both offline and online data. 

## Q learning parameters

17 States
3 Actions : Maintenance, Opportunities,Do nothing
delta_T = 5

alpha = 1 # learning rate
max_alpha = 1
min_alpha = 0
alpha_decay_rate = 0.01
discount_factor = 0.85  
num_episodes = 500 # Number of episodes

epsilon = 1  # Epsilon-greedy exploration rate
max_epsilon = 1
min_epsilon = 0.01
exploration_decay_rate = 0.01

max_step = 50

## conclusion
costs without RL
![11](https://github.com/mamad-hosn/Reinforcment-Learning-Maintenance-Policy/assets/90955072/c315d7c6-b2be-490f-b225-916526eb9de9)
costs with RL
![33](https://github.com/mamad-hosn/Reinforcment-Learning-Maintenance-Policy/assets/90955072/6a3cbad0-0c49-4ffa-a071-4dcaef5b2834)
![22](https://github.com/mamad-hosn/Reinforcment-Learning-Maintenance-Policy/assets/90955072/0af63d1d-b11a-4026-ac13-f4de797d5485)




