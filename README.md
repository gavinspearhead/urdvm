# urdvm
VM of URD

**Download link**

* https://drive.google.com/open?id=0B31CIayG7uzDTnZFT0JhVGtTZnc


**Instructions**

* Import the .ova file into Virtual box.
* Portmappings should be in place for port 80 to 8080 (http) and 22 to 2222 (ssh)
* Go to http://localhost:8080/urd/
* Login as 
*    username: urduser
*    password: password12
* Select the correct newsserver by clicking in the menu on admin/usenet servers; make sure the indexing checkbox for the selected server is set and priority is larger than 1. Disable all other newsservers (XS4all - Newszilla) is enabled
* Start URD by checking the red button on the top left (it will turn green after a bit, indicating the daemon process is running.
* You can now update spots under supply / spots, then actions / update spots. You can also index newsgroups under settings / newsgroups or subscribe to rss feeds under settings / rss feeds. The results will we shown under supply / group sets and supply rss sets respectively. 

You can login to SSH with these credentials if necessary
Username: urduser
Password: urd

Note: don't expose the VM to the internet or other users on the local network, before changing the passwords. In URD this can be done under settings/ preferences / login. Make sure to also change the SSH account by logging in using:
* ssh localhost -p 2222 -l urduser
* passwd urduser
