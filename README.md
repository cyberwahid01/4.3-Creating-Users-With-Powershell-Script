<p align="center">
<img src="https://i.imgur.com/9JmwJSF.png" alt="osTicket logo"/>
</p>

<h1>Active Directory: Creating Users With a Powershell Script 🪟</h1>
In this portion of the Active Directory lab I use a custom Powershell Script to add 10,000 new users into our previously created Domain. I go through the process of Running Powershell ISE as an Administrator, saving a script as a Powershell file, running the script and observing User creation. From here I confirm that the users were successfully added and then I test the operation by choosing one of the users at random to log into our Client Machine remotely.  

(Link Back to Main Project Contents Page is at the Bottom of this Repo)
<h2>Environments and Technologies Used</h2>

- Lenovo Ideapad 5 Pro 16gb AMD Ryzen 7
- Microsoft Azure Resource Group
- Microsoft Azure Windows 10 Pro version 22H2 - x64 Gen2 Virtual Machine
- Microsoft Azure Windows Server 22 Datacenter: Azure Edition - x64 Gen2 Virtual Machine

<h2>Operating Systems Used </h2>

- Local Windows 11 Home Version 21H2</b>
- Windows 10 Pro Version 22H2 Virtual Machine
- Windows Server 22 Datacenter: Azure Edition - x64 Gen2 Virtual Machine
  
<h2>List of Prerequisites</h2>

- Microsoft Azure Subscription
- Microsoft Azure Subscription Credit 

<h2>Installation, Setup, Resource Setup, Executing Functions</h2>
1. First we are using the Windows Remote Desktop Connection protocol to log into our client as our Admin user "Jane Doe"
</p>
<br />

<p>
<img src="https://i.imgur.com/lHtkLDH.png" alt="1"/>
</p>
<p>
2. Next we need to enable the users in our Domain to be able to remotely connect to the Client machine. We can do this by accessing the Remote Desktop settings and adding our Domain Users to the list.
</p>
<br />

<p>
<img src="https://i.imgur.com/mhxFUjN.png" alt="2"/>
</p>
<p>
3. Onto the stage of adding users into our Domain, we first need to open Powershell ISE as an Administrator. Locate Powershell ISE, right-click it and choose "Run as Administrator"
</p>
<br />

<p>
<img src="https://i.imgur.com/aOF4Zwy.png" alt="3"/>
</p>
<p>
4. We then need to go on to open a new script in Powershell ISE. This is where we will insert/load our script that will create our users within the Domain.
</p>
<br />

<p>
<img src="https://i.imgur.com/58iLqiI.png" alt="4"/>
</p>
<p>
5. Next we need to create and save a script file which we will load into the script window. The script for this operation has been provided in order to efficiently add the Users into our Domain.
</p>
<br />

<p>
<img src="https://i.imgur.com/LBrri6K.png" alt="5"/>
</p>
<p>
6. We then insert the script into Powershell ISE and we can see part of it displayed here.
</p>
<br />

<img src="https://i.imgur.com/7u4FUhQ.png" alt="6"/>
</p>
<p>
7. After inserting the script we then pressed the play button in the top toolbar to run the script. In the bottom window we can now see the users being created in real-time. 
</p>
<br />

<p>
<img src="https://i.imgur.com/m6NxLr2.png" alt="7"/>
</p>
<p>
8. Back in our Domain Controller, if we navigate into the "_EMPLOYEES" Organisational Unit, we can see that the script has successfully created 10,000 Users into this folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/pVUr8Lf.png" alt="8"/>
</p>
<p>
9. From our earlier screenshot showing the script, we can see that the script has automatically assigned each user the password "Password1". We will now use the displayed user with username "ful.wos" to simulate a log in to our Client with this user account. 
</p>
<br />

<p>
<img src="https://i.imgur.com/LaqfIei.png" alt="9"/>
</p>
<p>
10. Below is the login page showing a successful entry of the users account details and password.
</p>
<br />

<img src="https://i.imgur.com/8DA6JB6.png" alt="10"/>
</p>
<p>
11. From within the start menu, once we are logged in, we can see being successfully logged in as "ful.wos" who is in our domain.
</p>
<br />

<p>
<img src="https://i.imgur.com/WNyTta3.png" alt="11"/>
</p>
<p>
LINK BACK TO THE MAIN PROJECT CONTENTS PAGE - https://github.com/cyberwahid01/Azure-Compute-and-Networking
