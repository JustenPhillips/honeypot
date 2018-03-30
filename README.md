# honeypot
## Which Honeypot(s) you deployed<br>
I deployed a combination of dionaea, Kippo, Snort, P0f.
<br>
<img src="https://raw.githubusercontent.com/JustenPhillips/honeypot/master/Capture2.PNG"><br>
## Any issues you encountered?<br>
The instructions Codepath gave in the assignment were pretty straight forward.<br>
Only with gcloud trying to bill me for using too many CPU. <br>
Accodingly to their FAQ reguarding the free trial, we are limited to only 8...
<br>Not too much with the honeypot server itself.<br>
Downloading the sessions.json until I realize I was aiming at the wrong file path.<br>
In my SSH client after login into the shell I ran a `pwd` and `ls -lh` to check the filename and size.<br>
then from my local windows machine I ran.<br>
`gcloud compute scp mhn-admin:/home/user/session.json ./session.json`<br>
easy mistake but I'll write about it in case someone else has it.<br>

## A summary of the data collected:<br>
Here is some data gathered in the web interface from Kippo. <br>
Kippo is used to log brute force attacks and the entire shell interaction performed by an attacker.<br> 
You can find these under the charts tab.<br>
The following is a list of IP addresses that frequently attacked my honeypot. <br>
I ran a IPLOOKUP on the most frequent one and it traced back to Russia.<br>
<br>
<img src="https://github.com/JustenPhillips/honeypot/blob/master/attackers.png">
<br>
Here is a list of the most common password Brute Forced. 
<br>
<img src="https://github.com/JustenPhillips/honeypot/blob/master/topasswords.PNG">
<br>
Here is a list of the most common users Brute Forced. 
<br>
<img src="https://github.com/JustenPhillips/honeypot/blob/master/topusers.PNG">
<br>
Here is a combination of both.
<br>
<img src="https://github.com/JustenPhillips/honeypot/blob/master/usrpwd.PNG">
<br>
This is a real time map that display attacks by location as they happen.
After a few hours this is what my map begun to look like.
<br>
<img src="https://github.com/JustenPhillips/honeypot/blob/master/Capture.PNG">
<br>

## Exporting Data
please refer to the sessions.json file included in the repo.
