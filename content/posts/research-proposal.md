+++
title = "Research Proposal"
image = "/images/post/post-2.jpg"
author = "Katie Burgess"
date = 2022-03-14T05:00:00Z
description = "This is meta description"
categories = ["Proposal"]
type = "post"

+++

## Intro

    My area of research in my proposed project area is machine learning in
video games and the level of enjoyment players get from playing against a
model. My specific proposed idea is creating a machine learning model that
plays competitive generation 1 OU pokemon on a host website called 
'Pokemon Showdown'. I chose this website because it is a popular website 
tens of thousands of people regularly use, allowing my AI to have a 
regular stream of people to play against in order to learn what to do. I 
chose Gen (or Generation) 1 OU, as it has a group of regular team choices 
with typical move set pool, and no complicating factors such as abilities, 
items, hidden stats, etc. I think that this is an important project 
because the realm of video games is constantly evolving. A CPU opponent is 
not a new idea, but a complicated AI model has not been used in many 
formats besides games like chess. I think that video game companies will 
be moving towards using AI in their CPU, and so researching how much 
entertainment a player can get as opposed to a human opponent.

## Existing Literature

    This is not an entirely new concept in research literature. 
Ghasemi, Maryam, et al. "Design and Construction of Zana Robot for
Modeling Human Player in Rock-paper-scissors Game using Multilayer
Perceptron, Radial basis Functions and Markov Algorithms." ARO-The
Scientific Journal of Koya University 9.1 (2021): 67-76. discusses a
'rock paper scissors' game AI and the enjoyment players get while
playing against it as opposed to a randomizer, 
and the difference when the players know that they are against an AI. 
Norström, Linus. "Comparison of artificial intelligence algorithms for pokémon
battles." (2019). discusses the process of making the kind 
of model I want to create for my research project,though they do not 
extend this model to gauge player enjoyment in the way I want to. 
This is also seen in papers like (Lee, Scott, and Julian Togelius. "Showdown
ai competition." 2017 IEEE ),(Llobet Sanchez, Miquel. Learning complex games
through self play-Pokémon battles. BS thesis. Universitat Politècnica de
Catalunya, 2018.),(Rill-Garcıa, Rodrigo. "Reinforcement Learning for a
Turn-Based Small Scale Attrition Game."). This showed me that I would have
to pivot and add to the idea of simply building an AI model for this game.
Overall, there is already an idea of the basic effect machine learning has in 
player enjoyment, but not in the specific angle that I want to look into.
    This is the research gap that I want to cover in my senior comprehensive. 
I want to specifically find out what the effect on the level of enjoyment 
for players is when they play against an AI, and if there is an effect on 
win rate when the player knows the opponent is an AI (i.e. does the player 
try harder or not as hard when they know their opponent is an AI?). This 
seems to be present because possibly since this has been done in more 
simple games, no one has done this in the way I want to and specifically 
in the kind of game I want to do it in. The implications of this gap could 
be that there is no enjoyment difference, though I think that is a very 
relevant and important piece of information for the video game industry to 
keep in mind for the future of games. My solution to this gap is to create 
my own model, train it on 'Pokemon Showdown', and once it has an average 
or above skill level based on the website's ranking system I will hold an 
experiment where I have people play against the model and against each 
other and see if they feel the experience is more or less fun based on who 
they are playing against and if knowing their opponent is an AI changes 
anything for them in terms of choices or enjoyment.

## Methods

My research questions for this project are as follows:
    1. Does playing against an AI change player enjoyment?
    2. Does the AI win more or less based on player knowledge of the AI?
    3. How skilled at the game can the AI become?
These questions are very achievable for the project and all feed together 
in the overall structure of my research project. 
    The prototype that I have created will easily support my project. Like I 
have mentioned easier, I have many ideas of how this prototype will be 
able to assist in helping my AI become as good as possible though both 
training, testing, and documenting it's skill level. Since this prototype 
gives most of the code necessary to navigate through, open, and play a 
game, it will be very easy to just add the AI and run it through the site. 
In other words, I know that this prototype will support my project as it 
will make it easy to support my machine learning model.
    The experiment was a continuation onto my prototype. My research question 
was something I was thinking about since the beginning of my thoughts into 
my research topic: which team member do I start with? This is a much more 
crucial question than it seems. The pokemon that is sent out first is the 
one thing the AI is unable to control, as the pokemon that starts out on 
the field is based solely on the order in which your team is organized 
when you create it in the Team Builder. In order to give my AI the best 
chance of success as possible, I wanted to make sure I was choosing an 
optimal Pokemon for it to begin with. This caused my research to be as 
follows: 'Which pokemon should my team open with in order to have the best 
advantage?'.
    My original hypothesis as to the correct choice was either Starmie, 
Tauros, or Exeggutor. This is because all of these either have a type that 
isn't commonly able to be countered through the common choices or is able 
to apply pressure to the opponent through status conditions such as 
paralysis or sleep. While the other members on my team could be good 
choices as well, they were either defensive choices which are better to 
save for late game or have types that are more susceptible to super 
effective moves.
    In order to complete this experiment, I added onto my prototype in order 
to allow it to open the game and wait to get an opponent to see what they 
send out. Once the game is open, I would tally their choice and close the 
browser, then rerunning the program. I did this around forty to fifty 
times, collecting a solid amount of data for my decision. Based on the 
choices overall and a focus on the most common choices, including 
Alakazam, Starmie, Chansey, Rhydon, and Gengar, I was able to make my 
choice and complete my experiment.

## Experiment

    Using the data I collected from my experiment, I decided to choose Starmie 
as my starting choice. Starmie either has a super effective choice against 
the opposing choices or is able to apply pressure through the opponent not 
being very effective or the threat of a disadvantageous status condition. 
While there could be a new choice that becomes optimal through further 
reflection once the AI is being built, that is an easy change that I can 
make. The experiences I gained through working on this experiment will 
greatly help me complete this project and achieve my main goals for this 
research. This is due to the fact that through choosing a good starting 
choice the player can have a challenging match up, as well as giving the 
AI a better chance of winning any given match.
    I explained my results from my experiment using language that isn't 
game-specific in order to make sure that those unfamiliar with my chosen
game or format would still be able to follow my logic. I also showed the
graph of my data to show people the visual showing why I decided to focus
on certain popular choices. These can be used in my project to explain its
foundations by demonstrating that the data that can be gained from this game
is very easy to visualize and there is a vast amount of different stats you
can gather.

![](/images/post/Results.png)

    I displayed my work this way in order to make it visually clear how much more often
some popular choices were over others. I also did it this way as I believed it would
be easier to verbally explain the significance of these, as writing down the reasons
for different choice strategies would get complicated, cluttered, and distract from
the data in the graph.

![](/images/post/Experiment-Workflow.pdf)

    I displayed my workflow for the experiment this way in order to make it clear how I
was using my prototype and collecting my data. I used colors in order to make the
steps pop against the background, making it more readable and easier to understand
for a general audience.

## Feasibility

    My research project has a manageable scope and is very feasible. I believe 
that it will only take me between two and two and a half months to create 
and refine the code portion of my project, including the graphs I plan on 
creating after the completion of my player experience trial. If given more 
time, I had an initial idea to build multiple different models with 
different search algorithms in order to test if there was a skill level 
and enjoyment level difference between the different algorithms, though I 
now believe that is too broad for this time frame and complicates the 
experiment a bit too much. I am following my research question the whole 
way through, as I will be looking into what exactly is the effect of 
having an AI opponent on a player's experience in game.
    The prototype greatly improved the feasibility of the overall research 
project. Going into this assignment, I was the most nervous about the 
practicality and the realistic possibility of my program being able to 
actually interact with the Pokemon Showdown website. While I technically 
could have my project not touch the website and manually put in the AI's 
selections myself, I felt like this would be way too much of a personal 
time and attention sink, as the amount of times I would have to run this 
program in order to train, test, and get it's skill level would be too 
high to be anything but a time waste. Being able to get a prototype 
working that is able to open the site, navigate through it's different 
pages, log into a account, write in the team that I selected to use, and 
start a match (the tasks that my prototype is able to complete) takes a 
lot of that stress off of my shoulders. 
    In terms of design and implementation, I chose to use Python as the language
I would be writing my code in. This is not only because I am most familiar
with Python, but also because the libraries and softwares I am using in order
to write my program all are based in Python themselves. For the prototype itself,
I employed Selenium, a web navigating library and Chrome Driver, an application/library
that allows you to open up a Chrome Browser for Selenium to navigate through.
These were entirely new softwares to me, and so I had the steep learning curve of
not only interacting with HTML for one of the first times in my life, as well
as learning these brand new libraries and implementing them in a short time to
navigate through many different pages. These were very useful libraries though,
and so having the prototype put the pressure on me to become proficient in them in
such a short time frame really improved my skills. The implementation for this prototype
is very straightforward and is admittedly somewhat spaghetti code. I did it this way as
the actual implementation of this prototype code may change depending on the way that I
need it to interact with the AI (currently I am considering have it be able to run the
prototype code with some additions allowing move input, opponent choice, and pokemon status
saving over and over again while saving the data it produces). If I was to organize it
well though, the different navigation commands would be split into functions, with a
better and more Pythonic implementation. The current implementation is currently
functional and reportable, which is what matters at this point of the senior comprehensive.
With Professors JJ and Maria as my readers, I have no doubt that they will help me make
sure that my code is organized in an efficient and professional way.

## Ethics

    Since my research project works with people without their knowledge, there are 
a multitude of ethical concerns. The first and foremost dealing with what I 
just said: the opponent does not know that their move choices are being 
collected for my research. I am currently trying to deal with that through 
multiple different choices for my implementation. My account I am using is 
current called 'research-proj', giving the opponent the ability to see that 
something is likely being researched in their match with my account. If they 
don't like the idea of that, they can very easily exit the match and start a 
new game with a different account. I am also not planning on giving my AI or 
web navigating program the ability to type in the chat during a game, 
preventing the AI from saying anything to the opposing player that they might 
find offensive or hurtful.
    Besides that concern, the only other current ethical problem with my project 
is making the game experience worse for my opponents. An example of this can 
be seen in my experiment: I was only checking for the pokemon that they were 
sending in. Hypothetically, I could open the game, grab that one piece of 
information, and then instantly close the match. While this could get my 
experiment done much faster, it would greatly disrupt the enjoyment of my 
opponents, causing problems for the website with player retention in the 
specific format that I am trying to run my experiment in. Not only could this 
cause problems for my research and the host website, it could effect players 
that I did not even play against, as they would then have to wait longer for 
matches if the players I collected data from quit playing on the site.
    In the case that new ethical concerns become apparent, I will reevaluate the 
methods I am using for data collection and make sure that I am either not 
effecting the opponent's enjoyment of the site, or improving it for them.

## Conclusion

    There are very clear next steps in order to develop and eventually complete my 
research project for my senior comprehensive. These steps are as follows:
1. Access and store online bank of stored game history for the Gen 1 OU format
2. Build AI model and integrate it with the prototype I have already built
3. Train AI using the gathered game history mentioned before
4. Test and debug AI model
5. Let the AI run against real players on the site, checking in to check skill level of AI, tweaking possible improvements.
6. Lay out player experiment
7. Hold experiment and collect participant data
8. Create graphs using python library Plotly in order to organize and visually display collected data and it's result
9. Analyze result and explain why this might be the case
    Some of these steps will take longer, such as step 2 and 3, while some will 
only take a few hours, such as step 6 and 8. I believe that the work that I 
have completed in my Junior Seminar have more than prepared me to take on the 
task of this project. Like I previously mentioned, I believe that the Selenium 
web scraping that I completed for my prototype is the hardest thing that I 
will have to do for this project, and with that being almost completed the 
project should be easy in technical terms besides the specifics of creating 
the machine learning model, the meat of the technical application for this 
project. Through summer research experiences, I have already created models 
using Plotly, so that will be a lot easier for me moving forward. On top of 
this, as Pokemon is a game I have known for a while now, understanding the 
game logic and why things might be happening the way they do will assist me 
greatly with making sure the model is following proper game logic and 
competitive theory. Overall, this is a project that I am very passionate about 
and I am looking forward to possibly continuing with this even if it isn't 
through a senior comprehensive class.