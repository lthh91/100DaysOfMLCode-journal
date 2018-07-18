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

<h3>Day 7 - Saturday, July 14th, 2018 </h3>
<b>Today's Progress:</b> Today I set up a neural net using keras. I only trained it with the 18 won games I had (although the Linux machine has given me 31 more since last night). There will be more adjustments coming in the next days, but basically the code is ready to run. I added a new library "HuyAIrunning.py" to store the playing class (the bot that used the trained model to play), and the original HuyAI.py was changed to HuyAItraining.py, as it was used to get training data. The AI seems to be still very "dumb" now, as it won none in 5 games, but I hope everything's gonna be better with more data.

On the next step: I think I will need to run it on some kind of server with the full dataset, as well as fine-tune the model. See you all tomorrow!

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai

<h3>Day 8 - Sunday, July 15th, 2018 </h3>
<b>Today's Progress:</b> Today is the World Cup final day, so I kind cut it short. Anyway, I trained the model with full data (using notebooks.csc.fi), and it seems to me that the bot really performed better than before, though there were still lost games. The biggest issue lies on the computing capacity, as I need to run tensorflow and keras in every iteration, the game gets very laggy on my laptop (whose GPU, unfortunately, is not supported by CUDA and Tensorflow). The trained model file is very heavy (>400 Mb) and can't even be uploaded to Github, but with the data I provide, you can get a somewhat similar model as mine by running the file training-model.py.

I guess with the learning purpose, this project was a success, though I am very sure I can improve it way further if I have access to better hardware. I think I will take on with a new project and maybe come back to this one in a more suitable time.

<b>Link to work:</b> https://github.com/lthh91/Starcraft-Python-AI---Huy-Mai

<h3>Day 8 - Wednesday, July 18th, 2018 </h3>
<b>Today's Progress:</b> After finishing the last project, I still had my mind on it for awhile, and couldn't decide what to do next. In the end, today I decided to make some small projects, that makes myself familiar with the OpenAI Gym library, the library that I was working on in day 1. I now finished the very first environment, the cartpole, which simply contains a plank with a ball on it. Your task is to balance the plank, so that the ball stays on it as long as possible. Granted that this project is a much easier version of what I did in StarCraft AI project, the fundamentals are the same, and since it requires much less computing resources, the result is much easier to observe: In my latest test run, after a simple neural net training, the average score increased from 22.3 to 192.3.

In next few days, I will apply the same logic (and maybe some other algorithms) with other environments in OpenAI Gym, as I started to feel comfortable with the environment. I also have some ideas to improve the StarCraft AI project, so even though I said I would not come back to that in a near future, who knows :))

<b>Link to work:</b> https://github.com/lthh91/OpenAI-Example
