<pre id="taag_font_DeltaCorpsPriest1" style="float:left;" class="fig-ansi" contenteditable="true"> </pre>

![License](https://img.shields.io/github/license/wolf-project/DotfilesLinux)
# My Arch Linux Dotfiles
## i3WM,Bumblebee_status,nitrogen and Termite


![I3][screenshot1] 
![I3][screenshot2]

[screenshot1]:https://github.com/wolf-project/DotfilesLinux/blob/master/Screenshots/2021-03-10-195310_1366x768_scrot.png
[screenshot2]:https://github.com/wolf-project/DotfilesLinux/blob/master/Screenshots/Arch-logo.png

# How it Works ? 

<strong>pacman</strong> -S `i3` `i3blocks` `dmenu` `lm_sensors` `nitrogen` `termite` 

yaourt -S ttf-inconsolata ttf-font-awesome ttf-dejavu terminus-font-ttf terminus-font lemonbar-git i3-gaps-git
	
$ git clone git://github.com/wolf-project/DotfilesLinux

$ unzip DotfilesLinux.zip

Move to you directorie <strong> /home/your-user/.config/i3/ </strong>  or <strong>/root/.config/i3/</strong>

Edit the i3 configuration (config) on /home/your-user/.config/config or /root/.config/i3/config
  
  add this command on you i3 "config" 
  
  <strong> 
	
	bar {
	status_command = <path to bumblebee-status/bumblebee-status> -m <list of modules> -p <list of module parameters> -t <theme>
	}
</strong>

# Usage
## Normal usage
In your i3wm configuration, modify the *status_command* for your i3bar like this:

```bash
bar {
	status_command <path to bumblebee-status/bumblebee-status> \
		-m <list of modules> \
		-p <list of module parameters> \
		-t <theme>
}
```

