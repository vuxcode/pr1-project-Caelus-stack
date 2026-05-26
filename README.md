[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/F4JWjZ9e)
# Project Instructions
Follow the instructions here: https://vuxcode.netlify.app/new/pr1/lessons/major-project-brief/

REMEMBER TO "COMMIT" YOUR CHANGES REGULARLY TO SHOW HOW YOU HAVE BUILT THIS PROJECT! 

The final program is not the goal! The aim of the project is to show how you have developed your program, the steps you have taken and the problems you have solved!

# Project Notes

Some of the things i learned more deeply:

Use arrays to store cards and hands.
Use objects to represent cards with rank, suit, and value.
Use loops to create several decks of cards.
Shuffle an array.
Use functions to split the program into smaller parts.
Handle special blackjack rules, such as aces being worth either 1 or 11.

Some problems I solved during the project:

I used many "console.log()" messages to test if the functions worked correctly before adding more alerts for the player.
Cards became undefined because "drawnewcard()" did not return the drawn card correctly. I fixed this by using return newcard.
My for loop in "calcHandValue()" had a mistake when I first wrote it. I fixed the function so it can loop through every card in a hand and add the values.
Aces were always worth 11 at first. I changed "calcHandValue()" so aces can count as 1 if the hand would otherwise go over 21.
I had to split the game into different functions to make it easier to test and understand.

The program is still text-based, but it is playable. A possible future improvement would be to add buttons and show the game information directly in the web browser instead of only using prompts and alerts.

# Project Summary

This project is a text-based Blackjack game written in JavaScript. The player starts with 1000 dollars and can bet money each round. The game creates a shoe with six decks of cards, shuffles the shoe and deals cards to the player and dealer.

The player can choose to "hit" or "stay". If the player chooses hit, they draw another card. If the player goes over 21, they bust and lose the round. If the player chooses stay, the dealer takes their turn. The dealer draws cards until the dealer reaches or beats the player's value, or until the dealer busts.

At the end of each round, the program checks who won and updates the player's bank. The player can then choose to play another round or stop the game. The game also ends if the player runs out of money.

The main functions are:

"buildnewshoe()" creates the card shoe.
"shufflearray()" shuffles the cards.
"drawnewcard()" draws one card from the shoe.
"startround()" starts a new round and asks for a bet.
"playerturn()" lets the player choose hit or stay.
"hit()" gives the player one new card.
"stay()" ends the player's turn.
"dealerturn()" controls the dealer's actions.
"calcHandValue()" calculates the value of a hand and handles aces.
"checkwinner()" decides who won the round.
"startgame()" controls the full game loop.

# User Guide

Open the `index.html` file in a web browser. The game starts automatically.

When the game starts, the player begins with 1000 dollars. The program will ask how much money the player wants to bet. The bet must be a number greater than 0 and cannot be more than the money in the bank.
After the bet is placed, the player receives two cards and the dealer receives two cards. The player can see their own hand value and one of the dealer's cards.

when asked what to do you either write hit or stay.
hit - draw another card
stay - stop drawing cards and let the dealer play.

if the player gets a handvalue over 21, the player busts and loses. if the player choose stay, the dealer plays. then the game checks the winner and updates the player bank.

after each round the player gets a choice, to play another or stop playing.
yes - another round
no - game over

the game stops when either, player chooses to stop or have no money left in bank.