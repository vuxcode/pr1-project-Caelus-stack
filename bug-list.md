# Bug List

> Make a list of the things that don't work as expected. Keep a list of things that you have fixed and try to document how you solved them.

1. When I first used "drawnewcard()", the cards in "playerhand" and "dealerhand" became undefined. the function had "return;", so it did not store the card in a variable when it was drawn. it was later fixed when i added 
return newcard; (bruteforcing)

2. at first the calcHandValue crashed. beacuse of the drawnewcard bug this also didnt work due to undefined problem. this was fixed as soon as problem no.1 was fixed.

3. the calcHancValue also had a problem with the for loop syntax. it was later fixed with the calcHandValue(hand);

4. i wrote gameactive == false instead of gameactive = false...

5. most of the bugs that happen was beacuse i tried new things like objects and functions that start other functions. learning objects really helped with what is shown to the player and calculating the value. After a while when i extenden the use of console.log i really saw the use of that command and i helped a lot. will use this much more in future projects.
