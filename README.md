HDMI output for NeoGeo MVS
==========================

Summary: The digital video and audio outputs from the Neo Geo MVS are tapped off before going through the DACs. Instead an FPGA reads the data and outputs the signal over HDMI forming a direct digital to digital connection.

_This project might also be notable in that it's one of the very few (that I know of) that features working audio over HDMI._

<a href="http://www.youtube.com/watch?feature=player_embedded&v=humublc3Fqs
" target="_blank"><img src="http://img.youtube.com/vi/humublc3Fqs/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="480" height="360" border="10" /></a>

The FPGA generates the HDMI video signal with data islands to embed the audio. It also controls the clock of the Neo Geo MVS so it can produce the exact 720x480p at 60fps timing that the HDMI specification demands. See the [notes](Notes.md) for more details.

*Nb. The code was originally based off the HDMI/DVI sample code from [fpga4fun.com](http://www.fpga4fun.com/HDMI.html).*
