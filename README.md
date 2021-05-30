# ApertureTerminal
Settings to make your Windows-Terminal Portal 2 themed!
The background is taken from Portal 2's files, and as I don't know about Valve's Copyright policies very well I've decided to not include the GIF on here unless I get granted permission to do that by Valve. 

# Inspiration
I made this based on the settings posted by reddit user [u/zushiba](https://reddit.com/u/zushiba "u/zushiba"), which were in turn based on those from user [u/runew0lf](https://reddit.com/u/runew0lf "u/runew0lf"). I'm a big Portal Fan myself so I couldn't pass this opportunity. [Here's my original Reddit Post](https://www.reddit.com/r/Windows10/comments/no7mg8/i_tried_to_make_my_windows_terminal_look_like/ "My Post").

# How to install:
0. (Install the Windows Terminal from the Microsoft Store if you haven't yet!)
1. Download the Image Files from here, and move them to ```%LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\RoamingState```
2. To obtain the GIF for the background, refer to the section **How to obtain the animated background**
3. Open the Windows terminal and open the settings menu by either pressing <kbd>CTRL</kbd> and <kbd>,</kbd> or by pressing the little drop-down menu next to the tab and selecting "Settings".
4. Press the "Open JSON-File" button in the bottom right of the settings Panel, and open it with an editor of your choice
![image](https://user-images.githubusercontent.com/23218251/120101803-3707db80-c148-11eb-9d28-97c768956fd0.png)
5. Paste the following code into the appropriate spaces in the JSON-File:
This goes into the Array ```"list": [```, don't delete any of the profiles in there, just paste this in front of the other profiles.
```
            {
                "acrylicOpacity": 0.5,
                "backgroundImage": "ms-appdata:///roaming/p2terminalbg.gif",
                "backgroundImageAlignment": "center",
                "backgroundImageOpacity": 0.5,
                "backgroundImageStretchMode": "fill",
                "colorScheme": "Aperture",
                "cursorColor": "#A66900",
                "cursorShape": "vintage",
                "experimental.retroTerminalEffect": true,
                "hidden": false,
                "icon": "ms-appdata:///roaming/aperture_transparent.png",
                "name": "Aperture",
                "tabTitle": "Aperture Science",
                "useAcrylic": true,
                "padding": "40, 24, 40, 24",
            },
```
This goes into the Array ```"schemes": [```, don't delete any of the schemes in there, just paste this in front of the other schemes.
```
        {
            "background": "#6F3D00",
            "black": "#A66900",
            "blue": "#A66900",
            "brightBlack": "#A66900",
            "brightBlue": "#A66900",
            "brightCyan": "#A66900",
            "brightGreen": "#A66900",
            "brightPurple": "#A66900",
            "brightRed": "#A66900",
            "brightWhite": "#A66900",
            "brightYellow": "#A66900",
            "cursorColor": "#A66900",
            "cyan": "#A66900",
            "foreground": "#A66900",
            "green": "#A66900",
            "name": "Aperture",
            "purple": "#A66900",
            "red": "#A66900",
            "selectionBackground": "#A66900",
            "white": "#A66900",
            "yellow": "#A66900"
        },
```

6. Done! Enjoy your Terminal's new look!
![image](https://user-images.githubusercontent.com/23218251/120101673-7eda3300-c147-11eb-8635-3a34ab491886.png)

# How to obtain the animated background
0. (Install Portal 2 if you haven't yet)
1. Navigate to ```C:\Program Files (x86)\Steam\steamapps\common\Portal 2\portal2\media\sp_credits_bg.bik``` and copy this file to a convenient location.
2. Open [Aconvert Video](https://www.aconvert.com/video/ "Aconvert Video") in a browser of your choice, and upload the file to the service.
3. Click on Options and choose ```Change Size, bitrate or frame rate```
4. Choose the following settings:
```
Target Format: GIF
Video Size: 1920x1080 (1080p)
Video bitrate: 512k
Frame Rate: 60 or 30 (Up to you, 60 looks smoother)
Video aspect: Do not change
```
![image](https://user-images.githubusercontent.com/23218251/120102548-d37fad00-c14b-11eb-8ee4-e94fb15bf3d5.png)
5. Click "Convert Now!" and download the converted file.
6. Rename the file to "p2terminalbg.gif" and place it inside of ```%LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\RoamingState```
7. Done! Everything should be in working order now!
