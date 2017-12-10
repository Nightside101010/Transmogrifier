# Transmogrifier   v0.1.1
KSP Generic Part Resizer

The transmogrifier is SUPPOSED to resize all your parts. And it mostly works. The ultimate goal of this mod is to provide a light-weight, generic part resizing, in much the same way that SMURFF corrects masses of parts.
HEAVILY inspired by Kerbas Ad Astra's masterpiece of ModuleManager configury, SMURFF, and indended to complement its effects.

TRANSMO-

GRIFIER

[REQUIRES MODULE MANAGER]
(Some features require SMURFF)

The transmogrifier is a magic box. Put something in, turn the dial and out comes...   ...   ...different sized parts!  

Currently the settings are configured to change stock parts to roughly real-life sizes (Mk1 parts are now 2m in diameter), but other scales are possible.

This is a work in progress do not use in an existing game, as this will break all inflight vessels and .craft files as well. I am posting the mod in this early state in the hopes of getting some feedback and help on things I'm stuck on or have not noticed yet.

WHAT IT DOES
-The basic patch resizes rockets to realish proportions (default setting) but doesn't change fuel capicities. This should play well in stock-sized solar systems up to 3.2x resized systems.

OPTIONAL EXTENSIONS
-Resize Internals (and kerbals too!) - This makes IVAs match external sizes.
-Full Tanks - Full thrust: Allows for a ultra-light realish experience, if you want to play in RSS or 10x resized systems. (Balacing is WIP.)

ISSUES
-Not tested with very many mods. Stockalike mods will probably be ok, mods that do anything fancy, such as Procedural Parts probably won't work.

-Stock Fairings work, but the truss structure is not resized.

-Internals are resized, inside kerbals are resized, is this a good thing or an abomination!!??!?

-Fuel capacity and thrust increased to realish volumes, but not fully sanity checked yet.

-ModuleLiftingSurface values are not scaled, because I don't know what they mean, any help explaining this module would be appreciated.

GOALS
-Allow a easier "kerbal-alike" experience on a real-life scale, without all the hassle of maintaining a Realism Overhaul install.
-Refine resource volume changes
-Make sure masses are reasonable
-Find any bugs or unintended features

FEATURES

If you need to exclude a part from resizing you can use this Module Manager patch.

@PART[MySpecialPart]:FIRST
{
	TransmogrifyExclude = true
}


CHANGES

v0.1.0 "Bigger and Beta"
	-Tank volume and Thrust changes require SMURFF by Kerbas-ad-Astra, not included.
	-General cleanup and documentation.
	-WIP compatibility for RSB and SSTU

v0.0.2 "Bigger Kerbals"
	-Modular, if you don't want a particular resize feature you can disable or removet the cfg and the rest should work. Just keep Transmogrifier.cfg
	-Fixed internal resizing. I've also increased size of kerbals... (but only when inside parts)... Is this a good thing?
	-Made Stock fairings look right. Still WIP to get the autotruss feature looking good.
	-Introduced FillErUp.cfg to put an appropriate fuel capacity in the bigger tanks, definitely needs balancing and sanity checking.
v0.1.1 
	-Refine patches
	-Check for MM 3.0.0 compatibility
