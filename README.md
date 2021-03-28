# move-to-next-monitor (Revisited)

Now the script does not only add screen width/height to window position 
but computes relative position on one screen and moves window to relative
position on other screen. Now the script works with monitors that are not 
the same size.

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


![image](https://user-images.githubusercontent.com/72152874/112764417-b540e800-9008-11eb-92b3-eb4742de321a.png)

## Dependencies

```
wmctrl
xdotool
xrandr
```
