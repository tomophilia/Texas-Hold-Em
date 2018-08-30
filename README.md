# Texas-Hold-Em
A Texas Hold Em poker game.  


User controls all players as of now.

Uses the Frenchdeck class from Fluent Python.

All other code is original.  

The main functions are:
game_of_poker() - Runs a hand and moves the button.

HandoPoker() - A hand of poker.  From posting small and big blinds, up to calling the winner.

action_round() A round of betting.  Will end once all players with a live hand have the same bet in front of them.

CallRaiseFold() - Once action is on a player, they can check or bet.  If there already is a bet, the player must call or fold.

rankthehand() - take a player hand and return an ID such that the hand can be compared to other hands. I.E. - [6,[14]] - which would be Aces Full.  The first number is the hand rank with straight flush being 8, four of a kind being 7, .... and high card being 0.  The second item is a list that includes info about the straight, two pair etc. such as which two pair, how high a flush etc.

gatherPot() - gathers all bets and adds them to the pot

Player methods:

deal_a_hand() - deal a player a hand of n length in case you want to play other games ie - pineapple, omaha.
final__hand_met() - returns the best hand possible out of player cards and the board.
place_bet() - places a bet.  Takes from the player bankroll.
