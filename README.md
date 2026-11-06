ARMS models a shop that sells perishable goods as a sequential decision problem. A pricing agent and an inventory agent cooperate, each with its own reward and safety masks, trained with MAPPO. The repository compares five RL algorithms with three grid-tuned classical rules under one protocol (5 seeds, equal budget), with ablations, unseen-shop tests, cross-play and sensitivity analysis. All data are simulated.

Results: a tuned (s,S) rule is best on the shop it was tuned for; DQN, Double DQN, PPO and MAPPO are within about 1% of each other. On shops with changed demand or shelf life, MAPPO holds up best (return 4,923 vs 3,343 for the rule).

Run: python final_tests.py, then python -m streamlit run app.py.
