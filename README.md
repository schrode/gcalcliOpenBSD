# gcalcli for OpenBSD
<A HREF="https://github.com/insanum/gcalcli"> gcalcli </A>tweaks &amp; notes for OpenBSD
+ Since there's no package maintained for gcalcli, pip is a solid option

If not already present, install py3-pipx (stand alone pip)  
<b># pkg_add py3-pipx</b>

If not already present, install Rust compiler  
<b># pkg_add rust</b>  

Install gcalcli via pip  
<b>$ pipx install gcalcli  

(Install runs ~15 min)  

Add to your $PATH:  

Bash
<b>$ pipx ensurepath  

Other Shells
add /home/[username]/.local/bin to $PATH 

From here, follow gcalcli instructions on OAuth setup (https://github.com/insanum/gcalcli/blob/HEAD/docs/api-auth.md)

Once client auth is set up as a project, the initial config will give a message similar to the following:  
Not yet authenticated.
Starting auth flow...
NOTE: See https://github.com/insanum/gcalcli/blob/HEAD/docs/api-auth.md for help/troubleshooting.
Now click the link below and follow directions to authenticate.
You will likely see a security warning page and need to click "Advanced" and "Go to gcalcli (unsafe)" to proceed.
Please visit this URL to authorize this application: https://accounts.google.com/o/oauth2/auth?other-OAuth-and-ClientID-and-ClientSecret-things-here  

<b> There may be a notice that Google has not verified this app, depending upon how the personal Goolge project for gcalcli is configured.  
