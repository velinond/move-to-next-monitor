# move-to-next-monitor (Revisited)

Now the script does not only add screen width/height to window position 
but computes relative position on one screen and moves window to relative
position on other screen. 
This script has not yet been tested on other setups, if it does not work, it might be needed to change the way it looks for connected monitors

## KNOWN BUGS: 
1) if the window is tiled, it will be moved however after it is untiled
it will return back to previous screen. This could be fixed by untiling it 
first moving and tiling it back the same way as this script deals with 
maximalized windows. However I did not find command or window property 
to un/tile window.
2) integer division errors

## Usage

* Download script to desired directory (~/.local/bin) 
* Make sure directory is in $PATH                     
* Add permissions (chmod 775 move-to-next-monitor.sh)
* Configure shotcut  Keyboard->Application shorcuts->Add 


![image](https://user-images.githubusercontent.com/72152874/112764885-cd196b80-900a-11eb-8564-f73d967b3454.png)


## Dependencies

```
wmctrl
xdotool
xrandr
```
