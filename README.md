# honeypot
Which Honeypot(s) you deployed
Any issues you encountered
A summary of the data collected: number of attacks, number of malware samples, etc.
Any unresolved questions raised by the data collected
Additionally, include a json export of the data you collected in the repo, instructions for which can be found in the next section.

Exporting Data
The submission for this assignment will require an export of the data collected from your honeypot(s). You'll want to leave the honeypots up and running a while -- the longer the better -- and then export the data at the end of the assignment and download it to your host machine.

To export the data to json, ssh into the MHN admin VM and run the following command:

$ mongoexport --db mnemosyne --collection session > session.json
connected to: 127.0.0.1
exported 12828 records
A new file, session.json, should be created in the current directory. You can download this file to your machine and check it into the GitHub repo you create for this assignment along with your README.md write up.
