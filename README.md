# Jellyfin-Announce
a simple python script to announce maintenance to all users currently active every 10 minutes until the final 5 minutes when it counts down every minute

the notification pops up in the bottom left of the client screen and works on most clients

#instructions
edit the sendit.py and change the options near the top of the file (ip address and api key for the jellyfin install, you can use the domain name if you like but ip address is my go to) save the file after you have made the edits

`sudo chmod +x sendit.py` 

then you can run the script using the following 60 minutes before you decide to do server maintenance 

`sudo python3 sendit.py`

then it will run for you, keep the window open for it to keep counting down.

you can run this in the background using this `nohup python3 sendit.py > output.log 2>&1 &`
