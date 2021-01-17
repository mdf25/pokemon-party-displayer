# Pokemon Party Displayer
Used to display your pokemon party in a web browser so you can add it to OBS in your live stream!

## How it works:
- Download the included HTML file and place it somewhere on your computer. Let's say it's here: ```C:/path/to/file/PokemonLoadout.html```
- In OBS, open up a new web source. Point the target to this file instead of a web address but add file:/// in front of the path like this: ```file:///C:/path/to/file/PokemonLoadout.html```
- Depending on what size you want it, set the size to either 1000 x 200 or 200 x 1000 pixels. This will be important later.

## Getting a party member to display:
Now that we have got the URL source imported you should see nothing so far. Don't worry, that's fine. Let's fix that.
- Assume we started the game with a Charmander. To add his sprite to your party, open up the URL source again, and on the end of the file path, add this: ```?party=charmander```
- Save the source and you should now see Charmander's sprite appear on screen.
- Say we caught a Pidgey. To add him, change the last part to ```?party=charmander;pidgey```
- Voilla! Pidgey is displayed!

## Getting pokeballs to display behind party members:
If you want a set of Pokeballs to display behind the party members, just add this: ```&pokeball=1```
You now should see 6 Pokeballs ready to house your team!

## Changing display from horizontal to vertical:
If you want the pokeballs to display vertically, add this: ```&display=vertical```
ALl done!
