# ⭕ ROwOng // Ring Viewer in HTML / Pie Chart or Ring Chart monitor
This repo is meant to act as a website, listening for messages, when it hears a valid message, it draws the rings or arcs.

<br>
<br>

# 💡 Main Idea
On Github (which is here), on this repo, goto "Actions", and select the newest action so that you can access the URL to the GithubPage <br>
In our other "Parent file", setup an iframe with the source or link linked to the URL of the GitHubPage <br>
Everytime when you want to update the ROwOng Viewer, you will post a Message to the iframe. <br>

<br>
<br>

# 🔧 Technologies
- HTML
- CSS
- Javascript
- GitHub Pages

<br>
<br>

# ✉ Posting Messages
the message is an array full with objects <br>
each object contains the following attributes :
- `opr` : operation, for now, the only available value is "ring", which means to draw a ring or arc
- `ri` : radius-in : inner radius in pixels
- `ro` : radius-out : outer radius in pixels
- `as` : angle-start : starting angle of the ring / arc, in degrees
- `ae` : angle-end : endding angle of the ring / arc, in degrees
- `co` : color : color of the ring / arc, rgba format
for now, all object is an "instruction" to draw a ring / arc

<br>
<br>

# ❓ How can this be used ?
on our Website, our Single Clock uses this repo : https://memo2007ultra.wixsite.com/m27u-g2010/clock <br>
Type in the duration you desire, press Reset, decide if the mode is "Timer" or "Stop Watch", then press "Count" <br>
and you can watch the Ring / Arc spin <br>
If you need to work with 2 files from the Webdev perspective <br>
There are 2 files in this repo :
- main.html : the one with the iframe
- index.html : the one which will draw the rings
