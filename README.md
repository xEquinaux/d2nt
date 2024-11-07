# D2NT [etal] and Cactus
### Servicing D2NT for 1.13 [primarily single player]

<hr>

There might be ways to make D2NT work for 1.14d, granted it might require another DLL that the one I had to dig out of GitHub to make this work (like it used to) in the first place. I tried a number of options including what came with the vanilla GitHub repo and only one weird combination worked. Basically I had to go find a 1.13-specific Etal repository sitting around and use that DLL. Thus why this is primarily limited to 1.13. Also that is why I included the Cactus binaries into this repo because, to be blunt, it's a pain finding out where all of these sources are. Plus the Cactus binaries were originally on some strange website I was weird enough to download from several years ago (when it was supposedly legit anyway--new resources and all). If you are wondering about legitmacy, the Cactus repo on GitHub has that link sitting around.

<br><br>

I've put this bot together more than once in the last several years, and yeah it's really annoying finding out all the old things I had to do to get it working. So here it is primarily for my own sanity.

<br><br>

### An Important Note 
#### A feature change in D2NT's single player botting

<br>

One thing worth mentioning is that I edited NTBot.ntj to accept ANY character index on the character select screen for single player. I don't know if that bricks the internal fidelity checking of D2NT (like if it checks if a file has changed or something), but the first 20 or so lines are encouraged as changeable anyway by it's own comments section. Basically this means more than one single player instance can be run at once. I'm weird and just wanted to get characters to bot for a while to see what's up. I had more than one character and using one virtual machine instance per single player character was completely stupid. Originally it just selects whatever is in the slot designated in the D2NT setup screen. In single player though, the latest-chosen character gets shoved into position one and reorients all the indices. So this changes that completely and instead selecting based on index, it selects the character position BASED ON CHARACTER NAME placed inside "Account Name". Bear that in mind.