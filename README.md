# The Settlers of Catan

## What is it?
The strategic board game The Settlers of Catan is a modern classic. Introduced in 1995, it has sold over 22 million copies worldwide. Learning how to play the game well requires an inherent understanding of probability, economics, game theory, and social interactions. 
<br>
This is my personal dataset of 50 4-player games I played on playcatan.com in 2014. Using the ingame statistics page and a spreadsheet, I logged starting position choices, the distribution of dice rolls, and how each player spent the resources they acquired by the end of the game. Note, of course, because this dataset only consists of my games, any analysis done is most relevant for games involving me…

## Questions I have considered:
In Caran1:
<p>
  1. How much luck is involved in winning a Catan game?<br>
  2. Does starting position matter? If so, what starting settlements lead to success from each position?<br>
  3. How much information on the eventual winner can be gained from starting position/settlements alone?<br>
  4. By looking at postgame stats, what leads to a win? Can these statistics be a guide for ingame strategy?
</p>
<br>
In Caran2: 
<br>
<p>
  1. Is the winner really lucky?<br>
  2. If yes, exactly how lucky is the winner?
</p>

## Data details/guide:
gameNum - each game I played has 4 corresponding rows, 1 per player.<br>
player - the starting position corresponding to each row<br>
points - how many points the player ended the game with (the game is won with 10 or more)<br>
me - the position I played during the game<br>
2, 3, …, 12 - how many rolls of each value occurred during the game (game is played with 2 dice)<br>
settlement1, settlement2 - each starting settlement is logged as 3 pairs of [number, resource]:<br>
L = lumber<br>
C = clay<br>
S = sheep<br>
W = wheat<br>
O = ore<br>
3G = 3:1 general port<br>
2(X) = 2:1 port for resource X<br>
D = desert <br>
production - total cards gained from settlements and cities during game<br>
tradeGain - total cards gained from peer AND bank trades during game<br>
robberCardsGain - total cards gained from stealing with the robber, plus cards gained with non-knight development cards. A road building card is +4 resources. <br>
totalGain - sum of previous 3 columns.<br>
tradeLoss - total cards lost from peer AND bank trades during game<br>
robberCardsLoss - total cards lost from robbers, knights, and other players' monopoly cards<br>
tribute - total cards lost when player had to discard on a 7 roll (separate from previous column.)<br>
totalLoss - sum of previous 3 columns.<br>
totalAvailable - totalGain minus totalLoss.<br><br>
EX: in game 1, player 1's first settlement was on a 6-lumber, 3-clay, and 11-clay.<br>
