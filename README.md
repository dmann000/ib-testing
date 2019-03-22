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

binary for IB gateway is  /home/ec2-user/Jts/ibgateway/972/ibgateway

I'm going to attempt an ubuntu instances with this youtube video to get a GUI:

https://www.youtube.com/watch?v=6x_okhl_CF4


got ubuntu installed and up.  I've run the following:

sudo apt update && sudo apt upgrade #command
sudo sed -i 's/^PasswordAuthentication no/PasswordAuthentication yes/' /etc/ssh/sshd_config
sudo /etc/init.d/ssh restart
sudo apt install xrdp xfce4 xfce4-goodies tightvncserver -y
echo xfce4-session> /home/ubuntu/.xsession
sudo cp /home/ubuntu/.xsession /etc/skel
sudo sed -i '0,/-1/s//ask-1/' /etc/xrdp/xrdp.ini
sudo service xrdp restart

# got rdp over putty... login screen pops up

# I'm unable to log in as ubuntu and don't see the same option as the video.
