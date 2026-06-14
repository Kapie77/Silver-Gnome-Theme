![silver1](https://i.ibb.co/Q3vYc8ft/screenshot.png)

# OTHER LANGUAGES
[Português](README.pt.md)

# HOW TO INSTALL THE THEME

## NECESSARY EXTENSIONS
To install themes in Gnome, you need some extensions that can be downloaded here: https://extensions.gnome.org/
- [Install Browser Extension](https://extensions.gnome.org/) - Allows you to install extensions via your browser.
- [User Themes](https://extensions.gnome.org/extension/19/user-themes/) - Load shell themes from user directory.
- Gnome Tweaks - You need this tool to manage themes. Install it through your distro's store or type the following in the terminal: ```sudo apt install gnome-tweaks```
- [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) - Allows you to place a background image on the lock screen.
- [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) - Allows you to customize the dock.

## INSTALLING THE THEME
Install all the necessary extensions above.

Go to the "home" folder and press Ctrl + H to view hidden folders (or check the option to view hidden folders), and create a folder named **.themes** and **.icons**.

Extract the theme .zip file, copy the extracted folder, and paste it into .themes.

Open Gnome Tweaks, go to Appearance, and under “Applications” and “Shell” select **RanmaTheme**, then press Alt + F2 to restart the shell and the theme will be installed.

### HOW TO CHANGE THE COLOR AND SIZE OF THE DOCK
To change the color of the dock, open Extensions, click on “Settings” in “Dash to Dock,” go to “Appearance,” and in “Customize dash color,” enter the color #cdd2d1.

To change the size, go to “Position and size” and under “Icon size limit,” enter 32px.

To change the opacity, go to “Appearance” and under “Customize opacity,” enter 80%.

### HOW TO INSTALL WALLPAPERS
Install the [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) extension from the Gnome Extensions website. Press the super key and open the Extensions application. In Lock Screen Background, click Settings, select the wallpaper, and you're done.
The images to be used as wallpapers are in the “images” folder.

### HOW INSTALL ICONS THEME
Install the “Captiva-2” theme: https://www.gnome-look.org/p/1511577

### HOW INSTALL THE CURSOR THEME
Install the “Twilight cursors” theme: https://www.gnome-look.org/p/1607387

# HOW TO MAKE NOTIFICATIONS APPEAR FOR TESTING
Type the command below into the terminal and a fake notification will appear.
<br>
```notify-send "Title" "Test message"```

# HOW TO TAKE A SCREENSHOT OF ANY AREA (SUCH AS THE LOCKSCREEN AND SCREENSHOT SCREEN)
Type the command below into the terminal, and a screenshot will be taken within 10 seconds:
<br>
```gnome-screenshot -d 10```

# THEME COLORS

| Color | Hex |  
|-----|------|
| Main green | #0ee6a7 | 
| Main gray | #cdd2d1| 
| Transparent RGB gray | rgba(205,210,209, 0.8) |
| Transparent grayish white in RGB | rgba(255,255,255,0.91) |
| Dark green | #096d49 | 
| Lighter green/blue (from his glove) | #4bfffe |
| White from the panel | rgba(255,255,255,0.75) | 


Cor do switch (o botão de on e off):
```bash
switch:checked {
```

The blue color when you right-click on the workspace and hover over the options is in:
```bash
menu menuitem:hover, .menu menuitem:hover, .context-menu menuitem:hover {
```

Color of the dots used to mark an option (like in settings -> fonts, where there are options to mark dots:
```bash
check:checked, radio:checked {
```

The blue color when you click on settings, for example, and the option clicked has a background color is in:
```bash
row.activatable:selected {
```

e aqui:
```bash
.view:selected:focus, .view:selected, .view text:selected:focus, textview text:selected:focus, .view text:selected, textview text:selected, iconview:selected:focus, iconview:selected, flowbox flowboxchild:selected, modelbutton.flat:selected, .menuitem.button.flat:selected, treeview.view:selected:focus, treeview.view:selected, row:selected, calendar:selected {
```

Selection buttons like Left or Right of Settings -> Window Titlebars:
```bash
notebook > header > tabs > arrow:checked, button:checked {
```
