# Transmogrifier
KSP Generic Part Resizer

The transmogrifier is SUPPOSED to resize all your parts. And it mostly works. The ultimate goal of this mod is to provide a light-weight, generic part resizing, in much the same way that SMURFF corrects masses of parts.
HEAVILY inspired by Kerbas Ad Astra's masterpiece of ModuleManager configury, SMURFF, and indended to complement its effects.

TRANSMO-

GRIFIER



The transmogrifier is a magic box. Put something in, turn the dial and out comes...   ...   ...different sized parts!  

Currently the settings are configured to change stock parts to roughly real-life sizes (Mk.1 parts are now 2m in diameter), but other scales are possible.

This is a work in progress do not use in an existing game, as this will break all inflight vessels and .craft files as well. I am posting the mod in this early state in the hopes of getting some feedback and help on things I'm stuck on or have not noticed yet.

Currently fuel capacity is unchanged so these are only "balanced" in a stock game, but this will change after I can fix a few other issues.

ISSUES
-Not tested with mods at all. Stockalike mods will probably be ok, mods that do anything fancy, such as Procedural Parts probably won't work.

-Stock Fairings do not work yet, I need to figure out how the fairing module works.

-Internals are not resized. Not sure if this is possible.

-Does not change fuel capacity yet.

-Some of the older stock parts don't resize because they use a legacy method of defining the model and scale. I've kludged this to work on some of the Squad parts, but 

-ModuleLiftingSurface values are not scaled, because I don't know what they mean.

GOALS

-Add tank capacity scaling so tanks have an appropriate amount of fuel for various system sizes.

-Integration with SMURFF and/or Sigma Dimensions to provide a light-weight realism mode.

FEATURES

If you need to exclude a part from resizing you can use this Module Manager patch.

@PART[MySpecialPart]:FIRST
{
	TransmogrifyExclude = true
}


