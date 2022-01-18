# How to secure your SSH server
**Over the basics** I have collected some ideas and advices to make more secure you SSH server:

> (Any of the links isn't sponsored, I just found some examples.)

The numbers are not ranking, I just used them instead of points. 

## 1. Do not use the default port
Use a 5-digit port instead

## 2. Use the default port for an endlessh
More details: https://www.youtube.com/watch?v=SKhKNUo6rJU&ab_channel=Wolfgang%27sChannel

## 3. Use private key instead of password
And store it secure, like a password. 

## 4. Use MFA
An article can be written about it, and fortunately it is written: https://www.digitalocean.com/community/tutorials/how-to-set-up-multi-factor-authentication-for-ssh-on-ubuntu-18-04
  
## 5. Disable the root account access with SSH
It makes the hacker's job harder, if the he/she had to guess the (root) username too.

## 6. Do not run any other server services as root (if it's possible)
If a hacker can get into a service which is running as root, the hacker got a root access too.

## 7. Run everything in a separate Docker
Started from the previous section, if there is an exploit in a service, a hacker potentially can harm the whole system. The docker helps on this problem, and can harm only a container (except the Docker has an unfixed exploit too).
  
## 8. Make everything up to date
If it turns out, that something in the system has an exploit (0-day), hopefully the developers would trying to fix, or mitigate that and publish a new version of the program. But if you do not update, the threat will increase, because not just a new version of the program will published, but the exploit too. (https://www.exploit-db.com/)
Even from the previous section, this program can be the Docker.

## 9. Use fail2ban
It's also makes the hacker's job harder. More information: 
  

## 10. Use GeoIP with iptables
Instructions: https://docs.rackspace.com/support/how-to/block-ip-range-from-countries-with-geoip-and-iptables/

  

## 11. Pentest your network
You can do it in your own, with the help of a video, for example: https://www.youtube.com/watch?v=80vIin4xGp8

Or you can use a tool, which may wouldn't be such precise, for example: https://www.bitdefender.com/solutions/home-scanner.html

  

## 12. Run automated configuration check
Based on more eyes see more, you can use an automated config checker. Maybe that's find something over which your attention has slipped. Or it is really useful if you are a beginner.

You can search for in the net, and build your's too.
An example, that I found: https://github.com/gakowalski/linux-admin/blob/master/automated-configuration-check.md

## 13. "Never settle"
Always train yourself. Security is process, not a status.

---
Feel free to extends this note or correct inaccurate things, and look back in the future. 
