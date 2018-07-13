# 100DaysOfMLCode-journal
This is an ongoing log of my 100 days of Machine Learning challenge

#100DaysofMLCode

<h3>Day 1 - Sunday, July 8th, 2018 </h3>
<b>Today's Progress:</b> Got a basic understanding of Reinforcement Learning and made my first attempt towards it by generating a Q-learning table for a 4x4 Frozen lake environment (OpenAI Gym).

<b>Link to work:</b> https://github.com/lthh91/FrozenLakeQLearningTable-example </b>

<h3>Day 2 - Monday, July 9th, 2018 </h3>
<b>Today's Progress:</b> Today I created an AI that plays the game Starcraft. It is still pretty basic, and there has been no ML algorithm applied, but I guess it's acceptable, as there were many things to set up, which included installing a 30GB game.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai </b>

<h3>Day 3 - Tuesday, July 10th, 2018 </h3>
<b>Today's Progress:</b> My AI can now complete a game with quite good results. The strategy is still hard coded, but it already beat a Computer bot at Medium Difficulty. I expect to apply some kind of learning algorithm tomorrow.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai
<b>Link to video:</b> https://www.facebook.com/capital91/videos/1877572995599413/?notif_id=1531248924848114&notif_t=video_processed

<h3>Day 4 - Wednesday, July 11th, 2018 </h3>
<b>Today's Progress:</b> Applying machine learning into the AI is more complicated than I thought it would. I think part of the reason was that I do not have much knowledge of the game itself, so I only tried to make the machine fine-tuned those variables that I previously hard-coded using Q-Learning. Apparently, that did not make many differences, since there are quite a few other variables that I need to take into consideration to win such a complicatedly strategic game. I don't think I have yet enough knowledge (regarding the game, and regarding Reinforcement Learning) and patience to create that many variables, and I don't think my machine can even handle that much learning at once. I will try to find another solution tomorrow.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai

<h3>Day 5 - Thursday, July 12th, 2018 </h3>
<b>Today's Progress:</b> As I was stuck with the algorithm, I had a Google search and found Sandex's tutorial on StarCraft bot. He has a great idea to use OpenCV to recap the map at every iteration and randomize the attacking strategy, then save the result if the bot wins. Though he is temporarily stopping there, I think I understand his tactic. After gathering enough data, we can run a neural net to determine what to do based on the map. Brilliant!

I never had any experiences with OpenCV, but I think I will be able to gather enough information to run a simple neural net in a couple of days. The real challenge right now is to collect enough training data. I already played about 5 games, but my bot kept losing and my data folder is still empty. Sandex promised he would share his dataset once he's done collecting it, but it seems that he has not finished with that, either. I reckon that my original strategy is not good as his, so it takes a long time (or forever) for my bot to win simply by chances. I will try some more times, and if it does not go well, I will try to edit the original strategy.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai

<h3>Day 6 - Friday, July 13th, 2018 </h3>
<b>Today's Progress:</b> Today I was not productive at all. For some reason I woke up at 4am and could not go back to sleep, so I felt tired all day. Anw, I found that Starcraft has a headless version, which seems to run only in Linux (well, a headless version is the game without its front-end side, which made only AI possible to play it), so I spent my whole morning setting up the old 10-euro HP Compaq desktop in my house to run it (should've taken much less time if I didn't kept changing my mind towards to arrangement of the device). Anw, it is working perfect. After 100 games, my AI won 11 (not bad, in my opinion), and together with 7 games the AI won in the normal version yesterday, right now I'm having 18 games ready to train my model. I'm letting the AI run through the night for another 1000 games and see how it goes and will set up a classification algorithm (a neural net) with that data.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai
