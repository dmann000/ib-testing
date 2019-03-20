# ib-testing
testing capturing data from interactive brokers api

sudo yum update -y

sudo yum install xorg-x11-xauth -y

Sudo yum install xclock xterm -y

http://sourceforge.net/projects/xming/files/

From <http://houseofbrick.com/installing-oracle-software-prerequisites/> 

	Installed xming on windows
	
#xclock works!

Downloaded twsapi_macunix.975.01.zip from here:
https://interactivebrokers.github.io/#

Scp'd over to ec2

scp -i ~/donmann.pem ./twsapi_macunix.975.01.zip ec2-user@34.236.244.203:/home/ec2-user

Unzipped in homedir:

Unzip twsapi_macunix.975.01.zip

Download IB Gateway here:
	https://www.interactivebrokers.com/en/index.php?f=16457
	
Needed java:
	Sudo yum install java -y
	
Xwindow came up - couldn't read it…
	Clicked left button - went through install
	
	Clicked checkbox and button I couldn't read
	
Opened IB Gateway
