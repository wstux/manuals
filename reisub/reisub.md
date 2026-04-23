# REISUB

If a Linux machine locks up or freezes completely, use REISUB to restart it more gently than pushing the Power Button. 

Hold down `Alt` and the `SysReq` (`Print Screen`) keys, and then type `R` `E` `I` `S` `U` `B`, with 2-3 second delays between the key presses to give the commands a better chance to complete.

- `R`: Switch the keyboard from raw mode to XLATE mode
- `E`: Send the SIGTERM signal to all processes except init
- `I`: Send the SIGKILL signal to all processes except init
- `S`: Sync all mounted filesystems
- `U`: Remount all mounted filesystems in read-only mode
- `B`: Immediately reboot the system, without unmounting partitions or syncing


## Some mnemonics for REISUB:

Rise up (from the dead) if you're inclined to zombie movies
BUSIER backwards, as in The System is busier than it should be!
Reboot Even If System Utterly Broken.
Or the classic: Raising Elephants Is So Utterly Boring

## More info on all the `Alt`+`SysReq` functions

https://en.wikipedia.org/wiki/Magic_SysRq_key


### Sources:
- https://askubuntu.com/questions/4408/what-should-i-do-when-ubuntu-freezes
- https://blog.kember.net/posts/2008-04-reisub-the-gentle-linux-restart/
