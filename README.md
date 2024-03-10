# LevelDataArchive
Custom level data in a compressed, single-file archive, utilizing JSON and Copper files

## File Structure
To add an object to a level, a file with the name of that object will need to be made.

 - world // This folder is for objects that are stationary and have no logic to them, unless it is manipulated by a script
	 - model-01 //These files store an object type, object location, dimensions, and additional parameters based on type.
	 - model-02 //This will have an object type of "MODEL" and will need to be supplied a model
	 - model-03
	 - rectangle-01 //This will have a object type of "SHAPE" and will need to be supplied a shape type
	 - tri-01
	 - sphere-01
	 - comment.txt // Text files are ignored
 - actor
	 - actorname-01 //These files store an actor type, location, and additional parameters based on type
	 - actorname-02
	 - actorname-03
 - config
	 - playerstart //Specifies a player's starting position and any extra parameters that need to be supplied with a player
	 - startscript //Specifies a script that runs once on level init
	 - endscript //Specifies a script that runs once on level end/transition, before the next level init
 - script
	 - script-01.cop //Scripts that handle any non-actor based logic that needs to change based on the level
	 - script-02.cop
	 - script-03.cop
