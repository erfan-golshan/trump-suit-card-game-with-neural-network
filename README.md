# trump-suit-card-game-with-neural-network

Trump suit card game(Hokm) with neural network
“Dream land” mobile game application
“Dream Rain” game company
Erfan Golshan Artificial intelligence maker and game designer

Introduction
Today, machine learning and artificial intelligence have made a significant impact on technology and our daily lives, and they can also be used well to reduce complex tasks and heavy calculations to some extent or make them completely accessible. Meanwhile, artificial intelligence based on neural networks has had a tremendous impact and has helped a lot in the advancement of technology and science. In this article we are going to train a neural network AI to play a card game.

About this card game
In the trump suit card game (known as Hokm) cards randomly distributed among the players. The first player to get an ace can define the trump suit (this person is known as Hakem). Each player takes 5 cards at a time in the first turn. The dealing begins with the Hakem and continues anticlockwise. Right after Hakem receives his 5 cards, he must order up the trump suit. Cards are dealt out in 2 other turns until each player takes 4 cards. Ace has the highest value, followed by King, Queen, Soldier, and numbers. The trump cards are the most valuable of all. Hakem leads to the first trick. Each player in turn must follow suit. The highest number take the trick. Cards are collected from the ground and become a score. The winner needs to get 7 scores to win a round. If a player holds no cards of the suit led, that player may play any card including any trump card.
As can be seen from the rules of the game, in each turn, we must consider the cards played, trump suit, the cards in our hand and also the suits that our teammate or opponent team doesn’t have. 

Our objective
Our goal is to build an unpredictable artificial intelligence. The higher goal is to make a robot of a person. It means to upload his game data to the robot and the robot will learn from him and then play like him.

Investigating the interpolation method
In this method, we give a series of points from the domain of an unknown function to the neural network and give the value of the function at that point as an answer. Then we train the network. Finally, the network takes the form of that unknown function and learns to relate the domain points to the solution points. Our problem is similar. In a situation, we need to extract the data of the cards in person's hand and give the card he played as an answer. Then, finally, when the network trained completely, we call it every turn and get the answer. If it has seen that situation before, it will give the exact answer, but if the answer was not in its dataset, because it has been learned, it will answer the interpolated value of that data. 

work with neural network
One thing to consider is that the cards must be sorted. That is, the data of each turn must be categorized so that irrelevant data does not enter the network. For example, if the ground suit is spades, then the cards with spades suit in the robot's hand have value, and the cards of other suits should not even be given as input. After classifying the data and categorizing them, we train the network. At first, for initial tests we enter the data manually.
Then we use the data set of one of the professional players for real training.

Testing the network
In this section, we trained the network in each subcategory and also compare it with the person's game (we used PyTorch library). The network finally reaches an accuracy value, but by examining the data that acted differently, we realize that, for example, 3 choices have the same value from the network's point of view, and it selects one. We also ask the professional players and see that they also have the same opinion between these 3 choices.
With more accurate classification of data, the performance and responsiveness of the network increases.

The result of the game in the format of 4 players
Below we see the game result of this learned robot. All four players are the same robots.
*
The license of the code for the neural network and the results belong to the Dream Rain game company.
