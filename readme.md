# XnauiMUD

![GitHub repo size](https://img.shields.io/github/repo-size/NathanNuckels/XnauiMUD)

![GitHub last commit](https://img.shields.io/github/last-commit/NathanNuckels/XnauiMUD)

I have been trying to make a MUD for a WHILE now and I have finally found my mistake.
I was useing the waterfall workflow. I did some experamenting and I much prefer the agile workflow.
That means that I will make tiny changes to the code while still keeping it runnable instead of
dumping a load or garbidge code all at once and trying to fix it.

`Usage: java -jar target/XnauiMUD-0.0.1-INDEV.jar`

If the assembly plugin fails for some reason, try this:

`Usage: java -cp target/XnauiMUD-0.0.1-INDEX.jar com.phoenix.mud.App`

Javadoc is located in the reports tab of the site (target/site)

# TODO

Note to self: Take this with a grain of salt or you will will never finish!
- [x] Edit POM
	- [x] Add javadoc plugin
	- [x] Add assembly plugin (to make the jar file auto run)
- [ ] Create Main loop
	- [ ] create InputParcer
	- [ ] create Intro
- [ ] Create package room
	- [ ] Room
	- [ ] DefaultRoom
	- [ ] make the player keep track of what room its in
	- [ ] make the player start in DefaultRoom
- [ ] Create player package
	- [ ] Player
		- [ ] Health
		- [ ] Mana
		- [ ] Attack damage
		- [ ] id, NameString, desc
	- [ ] Tell the game to set the player to Player
	- [ ] Protogen
		- [ ] Has energy meter
		- [ ] Very smart
	- [ ] Kobold
		- [ ] very low max helth
		- [ ] spiky!
- [ ] Items
	- [ ] Base Item
		- [ ] Name, id, desc
		- [ ] placeible, sellible, sell price
		- [ ] droppable, key
		- [ ] stack ammount
	- [ ] Slot
		- [ ] holds an item
	- [ ] Container
		- [ ] holds slots
	- [ ] Tool
		- [ ] has attack damage
		- [ ] les you collect stuff
		- [ ] has duribility
		- [ ] Sword
			- [ ] dosnt collect stuff
			- [ ] has high attack damage
		- [ ] Axe
			- [ ] ok-ish attack damage
			- [ ] gets wood i guess
- [ ] Entitys
	- [ ] Base Entity
		- [ ] has health and atatck damage
		- [ ] can be a enemy or helpfull or neutral (use an enum for this)
		- [ ] name, id, description all that stuff
