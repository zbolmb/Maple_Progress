
----------------How to Run the Program----------------
MapleOpt_Full.jar requires the latest version of the Java Runtime Enviroment to be installed. You can install the latest version from httpwww.oracle.comtechnetworkjavajavasedownloadsjre8-downloads-2133155.html
Once the Java Runtime Enviroment is installed, you can simply double click the the MapleOpt_Full.jar file to run it.


----------------Inputs and Buttons and What They do----------------
Upper left side inputs of the program are the most important, these inputs will make the biggest impact and dictate what the optimizer returns as the best potentials, nebulites and legion configuration.
Note that changing any one of the following inputs or buttons will require you to hit the Calculate button again to see the updated configuration.

Upper left side inputs

	DMG- This stat can be calculated from the stat screen by subtracting any DMG% potentials you may already have on your Weapon, Secondary, or Emblem (WSE) and subtracting any DMG% nebulites you may have on your weapon or secondary.
	
	BOSS- This stat can be calculated from the stat screen by subtracting any BOSS% potentials you may already have on your WSE (Do not subtract the innate BOSS% already on weapons), subtracting any BOSS% nebulites you may have on your weapon or secondary, and subtracting any BOSS% you may have from covering the Legion boss squares.
	
	ATT- This stat cannot be calculated from the stat screen. You must find every source of ATT% you have from your class' passives and buffs. Reboot will always have at least 7% ATT (Echo and 3% ATT soul), Non-Reboot will always have at least 4% (Echo), though in most cases Non-Reboot will also have 7% ATT. (If you somehow cubed all 3 items to perfect bonus potential lines its possible a 7% Boss soul will give you more damage than 3% ATT soul)

	IED- This stat cannot be calculated from the stat screen, and you should NOT use the value provided by the stat screen under any circumstance (IT IS NOT YOUR TRUE IED VALUE). This can be calculated using the tool here httpsgmsmeta.comappsied.html (Do not include nebulites, potentials on WSE, or IED from covering Legion IED squares)

Middle left side buttons of the program

	SWAbsolabAU- This button is for if you are using, or plan on using, a weapon that is level 160 or higher.

	lvl 160+ Secondary- This button is for if your class has a secondary weapon that is level 160 or higher (Currently only applies to Dual Blades and Kannas).

	Kanna Class- This button is for if you are a Kanna. Kanna's secondary weapon that goes on Haku, only applies Magic ATT% to your character, so your ATT% when running the program should be include an additional 4% from a Magic ATT nebulite that Haku's fan should always have. The program will show only 1 nebulite to reflect the fact that Haku's fan should always have a 4% Magic ATT nebulite.

	Zero Class- This button is for if you are a Zero. The Program will show a secondary weapon and 2 nebulites, in reality you will only need 1 nebulite and you can ignore the secondary potential, as your weapon also counts as your secondary (potential and nebulite values are doubled from your weapon).

Bottom right side inputs of the program

	Boss Nebulite Value- This input can be changed to reflect the value of Boss nebulites you currently own, 2520% or 0% if you do not own any.

	IED Nebulite Value- This input can be changed to reflect the value of IED nebulites you currently own, 211815% or 0% if you do not own any.

	Legion Points for Boss and IED- This input is the total amount of Boss and IED squares you can cover on the Legion board (40 Boss squares max and 40 IED squares max). Do note however that crit damage is the most important stat from the Legion board and should be maxed before Boss and IED.

Bottom buttons of the program

	Calculate- This runs the program and calculates the best potential, nebulite and Legion configuration to maximize damage against 300% PDR bosses.

	Include Bpot- This button makes the program include bonus potentials in the calculation. Note that this requires much more memory and time to run.

	No 3 Line ATT Bpot- This button forces the program to ignore bonus potentials consisting of 3 lines of ATT.

	No 3 Line ATT- This button forces the program to ignore potentials consisting of 3 lines of ATT.

	Exit- Closes the program.

Middle Right side input
	
	Final damage tolerance for other configurations- This input is for how much worse you want to allow other configurations to be compared to the most optimal #1 configuration. They will be sorted in descending order of best to worst configurations. Note that setting this value very high will cause the program to run slow as it collects all the other configurations.

Bottom two text boxes
	
	Left text box- This shows your #1 best configuration after having hit calculate.

	Right text box- This shows your #2-X best configurations based on the value entered in Final damage tolerance for other configurations input. Possible to show no other configurations if none are within the tolerance.


----------------How to get Your Optimal Configuration----------------
1. Enter your class' values into DMG, BOSS, ATT, IED
2. Select the proper Middle left side buttons corresponding to special classes, and weapon and secondary item levels
3. Enter your Nebulite and Legion values in the Bottom right side inputs, or skip this step if they do not change
4. Select Bottom buttons if you are in Non-Reboot servers or do not wish to cube for 3 lines of att
5. Set the tolerance level in the Middle Right side input
6. Hit Calculate


----------------Reading the Output----------------
The program formats the output as main wep, sec, and emblem potentials, then bonus wep, sec, emblem potentials, then nebulites, then Legion points.
Under each WSE section the format is Legendary Line potential type, number Unique Line potential type
Under the Nebulite section the format is value of nebulite nebulite type nebs number you should use 
Under the Legion section the format is Legion type points number you should cover 

The program always selects the highest potential line for each type as follows

---Main Potential---
Boss
	Legendary line of Boss is 40% regardles off Weapon or Secondary levels
	Unique line of Boss is 30% regardles off Weapon or Secondary levels
ATT
	Legendary line of ATT is 12% for WSE under level 160 and 13% for WSE that are level 160 or over	
	Unique line of ATT is 9% for WSE under level 160 and 10% for WSE that are level 160 or over	
IED
	Legendary line of IED is 40% regardles off WSE levels
	Unique line of IED is 30% regardles off WSE levels

---Bonus Potential---
Boss
	Legendary line of Boss is 18% regardles off Weapon or Secondary levels
	Unique line of Boss is 12% regardles off Weapon or Secondary levels
ATT
	Legendary line of ATT is 12% for WSE under level 160 and 13% for WSE that are level 160 or over	
	Unique line of ATT is 9% for WSE under level 160 and 10% for WSE that are level 160 or over	
IED
	Legendary line of IED is 5% regardles off WSE levels
	Unique line of IED is 4% regardles off WSE levels

---Nebulites---
Self explanatory

---Legion---
Boss Points How many squares on the Legion board you should cover in the Boss section
IED Points How many squares on the Legion board you should cover in the IED section

----------------Advanced----------------
1. If your class has hyper points for passive that add DMG% or BOSS% to skills and those skills makes up a majority of your damage while bossing (50%), then you can take the weighted average of your DMG or BOSS with those passives for optimization.
2. If your class has hyper points for passives that add IED% to skills and those skills makes up a majority of your damage while bossing (50%), then you can take the weighted average of your IED with those passives for optimization. Additionally you can also do this for skills or buffs that allow you to ignore 100% IED or give additional IED on a cooldown (not 100% uptime or usage).