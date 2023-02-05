<p align="center">
<img src="https://i.imgur.com/Vv6aSXX.png" height="25%" width="25%" alt="vpn-pic"/>
</p>

<h1>VPN Setup and Usage</h1>
This walkthrough demonstrates how to setup a virtual private network in an azure virtual machine and the exercises that you can do to gain a better understanding of how vpns work and aswell as how remote protocol works.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h3> Operating systems used</h2>

- macOS (12.1)
<h2>Steps</h2>

<p align="left">
  Open a new browser on your physical computer and go to "whatismyipaddress.com" <br/>
<p>
<img src="https://i.imgur.com/GpJbz7m.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<p>
<p align="left">
  Entering the website, you should be able to view your IPv4 address and city location (mine is hidden of course). Open up notepad or textedit for mac and take note of them.  <br/>
<p>
<img src="https://i.imgur.com/nqlGI57.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Next step is to create a virtual machine in azure and connect to it via remote desktop <br/>
<p>
<img src="https://i.imgur.com/8DGdoT9.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Give the VM a name and make sure to place the virtual machine in a region that is not where you are physically located at. The VM will be running windows 10. <br/>
<p>
<img src="https://i.imgur.com/oCgBUNq.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
The size will be the standard running 2 virtual cpus. Create a username and password. After that check the confirmation box and click on review and create. <br/>
<p>
<img src="https://i.imgur.com/pX9wy4L.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
After it is done validating click create. <br/>
<p>
<img src="https://i.imgur.com/bhMXL2j.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Once the delployment is completed click go to resource. <br/>
<p>
<img src="https://i.imgur.com/tg9ww6d.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
We now have a public IP address for our virtual machine. That address will be the name we use for our VM. <br/>
<p>
<img src="https://i.imgur.com/sT77i3N.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
<p>
<img src="https://i.imgur.com/3d4uEGM.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
You should be able to log into the VM by using the username and password you created in the azure portal. <br/>
<p>
<img src="https://i.imgur.com/tkFgXPA.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
As you can see, when you go check for your IP address from within the VM, it is in the same location you set it to when you first created the VM in azure Take note of the IP address. <br/>
<p>
<img src="https://i.imgur.com/xLOezwt.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Now we will enable a vpn service to be used on the VMs IP address and observe what happens. You can sign up for Proton vpn to get access to their service. <br/>
<p>
<img src="https://i.imgur.com/K3bZ0WJ.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Head back over to the VM and log into your proton vpn account. Download the windows vpn client. Windows vpn client is simply an app that lets you connect to the vpn.  <br/>
<p>
<img src="https://i.imgur.com/kHZHHlM.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
To finish installing the client click next all the way through. Be aware that installing this may interupt the remote desktop connection for a few seconds.  <br/>
<p>
<img src="https://i.imgur.com/N21smEB.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Open the proton vpn app and log in with your creditials.  <br/>
<p>
<img src="https://i.imgur.com/1AyMF8b.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Connect to the Japan server. What this will do is create a tunnel from your VM to a Japanese vpn server, allowing us to browse through the the vpn in Japan.  <br/>
<p>
<img src="https://i.imgur.com/Da7gkpl.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Once you are connected go back to the whatismyipaddress website and observe how to IP address and location is different.  <br/>
<p>
<img src="https://i.imgur.com/MAWJMVt.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />

<p>
Since you are connected to a server in japan, everything should be in Japanese when browing the web.  <br/>
<p>
<img src="https://i.imgur.com/90VCmF1.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
</p>
<br />
