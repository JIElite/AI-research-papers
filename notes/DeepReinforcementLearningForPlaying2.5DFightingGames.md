It is a short paper proposed by the student from National Taiwan University, Taiwan. The main contribution in this paper are:
- Address the orthographic projection problem in 2.5D games.
- Release a OpenAI gym-like 2.5D learning environment based on LF2(game name). 

The interesting thing in this paper is that they addressed the visual ambiguity problem in 2.5D game, e.g., it's hard for agent to tell the accurate position when the character jumps from the floor.

The observation for agent are 4-stacked, gray-scaled screenshots which are similar to the settings of original DQN.The reward function is defined by the damage to enemy(positive reward) or the injury from enemy(negative reward)

Because of combo actions, it's helpful that they integrated A3C with LSTM to memorize the action sequence. 

In my opinion, if they can change the opponent's AI from rule-based AI to self-play may be more charming.