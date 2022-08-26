<h1>Setting Up a Honeypot</h1>


<h2>Description</h2>
In this lab, I learned to set up a honeypot. A honeypot is a computer system that is set up to trap cyberattackers who try to gain unauthorized access to information systems.
<br />



<h2>Environments Used </h2>

- <b>Kali GNU/Linux Rolling</b> 
- <b>Terminal</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar click Terminal: <br/>
<img src="https://i.postimg.cc/ry3NJW8p/Screen-Shot-2022-08-25-at-10-34-33-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the Terminal window type in "ifconfig"  <br/>
<img src="https://i.postimg.cc/662dy3dx/Screen-Shot-2022-08-25-at-10-36-39-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
Note down the inet IP addres for the eth0 router. It will be required for later use. <br/>
<img src="https://i.postimg.cc/Bn6Zn8Kx/Screen-Shot-2022-08-25-at-10-39-01-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window type in the following commands: <br/>
1. cd pentbox-1.8/ <br/>
2. ./pentbox.rb <br/>
(The Pentbox is a safety kit containing various tools for streamlining PenTest conducting a job easily) <br/>
<img src="https://i.postimg.cc/FFMnKwkG/Screen-Shot-2022-08-25-at-10-42-12-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window select option 2 for "Netwrok Tools" and then press enter.  <br/>
<img src="https://i.postimg.cc/Vs2nP80s/Screen-Shot-2022-08-25-at-10-46-33-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
In the terminal window select option 3 for "Honeypot" and then press enter.  <br/>
<img src="https://i.postimg.cc/NjjgNyGK/Screen-Shot-2022-08-25-at-10-48-29-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window select option 2 for "Maunal Configuration" and then press enter.  <br/>
<img src="https://i.postimg.cc/vBV9cqpw/Screen-Shot-2022-08-25-at-10-53-31-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window type 443 after the "insert port number".  <br/>
<img src="https://i.postimg.cc/Vk0YyxMw/Screen-Shot-2022-08-25-at-10-54-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />






<br />
In the terminal window whatever message you wish after "insert false message to show".  <br/>
<img src="https://i.postimg.cc/Wbk2xR0v/Screen-Shot-2022-08-25-at-10-57-14-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the terminal window type "y" for "save a log with intrusions".  <br/>
<img src="https://i.postimg.cc/2SW7q5vK/Screen-Shot-2022-08-25-at-10-59-23-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
at the stage press enter to save the log file in a default location .  <br/>
<img src="https://i.postimg.cc/qM31KQHw/Screen-Shot-2022-08-25-at-11-01-35-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Type "n' to disable sound for alerts about intrusions.  <br/>
<img src="https://i.postimg.cc/pLghFYxf/Screen-Shot-2022-08-25-at-11-04-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Now that our honeypot is set up to port 443 lets test it out by opening a web browser.  <br/>
<img src="https://i.postimg.cc/ZKHXnV8Q/Screen-Shot-2022-08-25-at-11-06-17-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />






<br />
In the web browser type in the "https://10.1.214.15" in the serach bar (The ip address is the one that we got from step two.  <br/>
<img src="https://i.postimg.cc/bNqvSyMw/Screen-Shot-2022-08-25-at-11-10-54-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
You will notice that error popped up.  <br/>
<img src="https://i.postimg.cc/Gt5SRhTx/Screen-Shot-2022-08-25-at-11-12-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Going back to the terminal window you will notice that our honeypot worked and detected our false intrusion.  <br/>
To stop the honeypot you simply pres Ctrl+C <br/>
<img src="https://i.postimg.cc/QCvGbqmD/Screen-Shot-2022-08-25-at-11-13-49-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />










  
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
