![image](https://github.com/user-attachments/assets/3378cb45-1c9d-4c28-ba78-510395693b2e)<h3>In this lab we will be creating a osTicketing system using a Virtual Machine on Microsoft Azure.</h3>

![osticket1](https://github.com/user-attachments/assets/d5426262-64ad-4457-b7fe-2fc65e12b4b4)
  - Our first step is to create a Virtual Machine that uses Windows 10 using Microsoft Azure, with a resource group named "osTicket" in order to easily identify our VM that will be hosting our ticketing system.
    <h4>Home > Search > Virtual Machines</h4>
    
  ![image](https://github.com/user-attachments/assets/150bbbda-0319-48c4-8c84-873b01f54569)
  - In step 2, we remote into our Virtual Machine using 'Remote Desktop Connection' by inputting the Public IP Address assigned to our VM with our created credentials.
    <h4>Search > Remote Desktop Connection > Computer = VM Public IP Address</h4>
  ![image](https://github.com/user-attachments/assets/bc9bb611-068a-4c27-bd0b-bb3afc3ee210)
  - Step 3 will include downloading the following zip file (https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&pli=1&authuser=1) then navigating through our control panel to enable IIS: <h4>Windows Search > Control Panel > Uninstall Program > Turn Windows Features on/off > [x] Internet Information Services</h4>
