# st - simple terminal
st is a simple terminal emulator for X which sucks less.


### Requirements
In order to build st you need the Xlib header files.


### Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

`make clean install`


### Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

`tic -sx st.info`

See the man page for additional details.

### Credits
Based on Aurélien APTEL \<aurelien.aptel@gmail.com\> bt source code.


## edit by rabuu
Font and colors can be defined in Xresources with:
* st.font
* st.color0
* ...
* st.color15
* st.background
* st.foreground
* st.cursorColor
* st.minlatency
* st.maxlatency
* st.blinktimeout
* st.bellvolume
* st.tabspaces
* st.borderpx
* st.cwscale
* st.chscale

### used patches
* [anysize](https://st.suckless.org/patches/anysize/st-anysize-0.8.4.diff)
* [boxdraw](https://st.suckless.org/patches/boxdraw/st-boxdraw_v2-0.8.3.diff)
* [delkey](https://st.suckless.org/patches/delkey/st-delkey-20201112-4ef0cbd.diff)
* [scrollback](https://st.suckless.org/patches/scrollback/st-scrollback-0.8.4.diff)
	* [scrollback-mouse](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-20191024-a2c479c.diff)
	* [scrollback-mouse-altscreen](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-altscreen-20200416-5703aa0.diff)
	* [scrollback-mouse-increment](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-increment-0.8.2.diff)
* [xresources](https://st.suckless.org/patches/xresources/st-xresources-20200604-9ba7ecf.diff)
