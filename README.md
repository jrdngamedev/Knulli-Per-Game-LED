# Knulli-Per-Game-LED
Per Game LED Script for use with TrimUI Brick and Knulli systems (Untested).

Before continuing, I am not responsible for any damage done to the device, use at your own risk.

This is just a script, its not hard-coded into the Knulli menu.
Place the script into userdata/system/scripts.

The script is fairly straight forward if you wanted to add your own per game LED settings.

Use an app like Notepad++ to edit the file.

Copy and paste a section like:

```
        elif [[ "$ROM_NAME" == *"Black"* ]]; then
                echo "Pokemon Black" >> "$LOG"
                knulli-rgb-led-daemon set 10 10 10
```

and just change what is between the "" e.g. "Black" to whatever KEYWORD is in your ROM filename and the 10 10 10 (RGB) values to whatever you want. Its probably best to go into the RGB settings on Knulli and tweak the values there to get the desired colour values. Technically speaking should work with all LED supported Knulli devices.

BEWARE: The longer the file, the longer it will take your game to load... I think. So delete games or keywords that you don't use.
