# reddit-wallpaper-rotator
Small shell script to keep a folder with fresh wallpapers using [RedditImageGrab](https://github.com/HoverHell/RedditImageGrab).

##Usage
Edit `config` to point to a wallpaper subreddit and specify a local wallpaper folder. Do not use an existing folder as the script will remove old files . 

Set run permissions with `chmod +x get-wallpapers` and `chmod +x cycle-wallpapers`. 
`get-wallpapers` replaces old images with new ones, `cycle-wallpapers` chooses a random image from the folder specified in `config` and sets it as a background image in Gnome and/or Unity.

Add  both scripts to your cronjobs, e.g. `get-wallpapers` once per week and `cycle-wallpapers` once per hour. If you use KDE, use the the system's desktop/folder view slideshow feature instead of `cycle-wallpapers`.
