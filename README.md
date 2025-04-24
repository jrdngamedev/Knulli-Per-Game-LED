# Knulli-Per-Game-LED
Per Game LED Script for use with TrimUI Brick and Knulli systems (Untested).

This is just a script, its not hard-coded into the Knulli menu.
Place the script into userdata/system/scripts.

The script is fairly straight forward if you wanted to add your own per game LED settings.

Use an app like Notepad++ to edit the file.

Copy and paste a section like:

elif [[ "$ROM_NAME" == *"Black"* ]]; then
      echo "Pokemon Red" >> "$LOG"
		knulli-rgb-led-daemon set 10 10 10	


and just change what is between the "" e.g. "Black" to whatever KEYWORD is in your ROM filename.

BEWARE: The longer the file, the longer it will take your game to load... I think. So delete games or keywords that you don't use.
