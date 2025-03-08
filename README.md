<h3>In this lab we will be creating a osTicketing system using a Virtual Machine on Microsoft Azure.</h3>

![osticket1](https://github.com/user-attachments/assets/d5426262-64ad-4457-b7fe-2fc65e12b4b4)
  - Our first step is to create a Virtual Machine that uses Windows 10 using Microsoft Azure, with a resource group named "osTicket" in order to easily identify our VM that will be hosting our ticketing system.
    <h4>Home > Search > Virtual Machines</h4>
    
  ![image](https://github.com/user-attachments/assets/150bbbda-0319-48c4-8c84-873b01f54569)
  - In step 2, we remote into our Virtual Machine using 'Remote Desktop Connection' by inputting the Public IP Address assigned to our VM with our created credentials.
    <h4>Search > Remote Desktop Connection > Computer = VM Public IP Address</h4>
    
  ![image](https://github.com/user-attachments/assets/bc9bb611-068a-4c27-bd0b-bb3afc3ee210)
  - Step 3 will include downloading the following zip file (https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&pli=1&authuser=1) then navigating through our control panel to enable IIS: <h4>Windows Search > Control Panel > Uninstall Program > Turn Windows Features on/off > [x] Internet Information Services</h4>
  
![image](https://github.com/user-attachments/assets/63d2657d-6412-4348-a863-98312896034b)
  - Step 4 includes creating a new folder in our **(C:)** drive named **PHP** and extracting our **zipped php file** into our created **PHP** folder.
    <h4>Browse > This PC > Windows (C:) > PHP</h4>
    
![image](https://github.com/user-attachments/assets/af8eced1-3bc1-4fcc-a10b-51c6a6595469)
  - For step 5, we will begin installing the rest of our applications in the following order:
    ```
        1) VC_redist
        2) mysql
            a. Setup Type: Typical & Launch
            b. Standard Configuration
            c. Password: root (NOT ADVISED SECURITY SETTINGS!)
    ```
