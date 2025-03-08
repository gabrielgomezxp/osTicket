<h3>In this lab we will be creating a osTicketing system using a Virtual Machine on Microsoft Azure.</h3>

![osticket1](https://github.com/user-attachments/assets/d5426262-64ad-4457-b7fe-2fc65e12b4b4)
  - Our first step is to create a Virtual Machine that uses Windows 10 using Microsoft Azure, with a resource group named "osTicket" in order to easily identify our VM that will be hosting our ticketing system.
    <h4>Home > Search > Virtual Machines</h4>
    
  ![image](https://github.com/user-attachments/assets/150bbbda-0319-48c4-8c84-873b01f54569)
  - In step 2, we remote into our Virtual Machine using 'Remote Desktop Connection' by inputting the Public IP Address assigned to our VM with our created credentials.
    <h4>Search > Remote Desktop Connection > Computer = VM Public IP Address</h4>
    
  ![image](https://github.com/user-attachments/assets/bc9bb611-068a-4c27-bd0b-bb3afc3ee210)
  - Step 3 will include downloading the following zip file (https://drive.usercontent.google.com/download?id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD&export=download&pli=1&authuser=1) then navigating through our control panel to enable IIS and CGI: <h4>Windows Search > Control Panel > Uninstall Program > Turn Windows Features on/off > [x] Internet Information Services > World Wide Web Services > Application Development Features > [x] CGI</h4>
  
![image](https://github.com/user-attachments/assets/63d2657d-6412-4348-a863-98312896034b)
  - Step 4 includes creating a new folder in our **(C:)** drive named **PHP** and extracting our **zipped php file** into our created **PHP** folder.
    <h4>Browse > This PC > Windows (C:) > PHP</h4>
    
![image](https://github.com/user-attachments/assets/af8eced1-3bc1-4fcc-a10b-51c6a6595469)
  - For step 5, we will begin installing the rest of our applications in the following order:
<br></br>
    ```
        1) VC_redist
        2) mysql
            a. Setup Type: Typical & Launch
            b. Standard Configuration
            c. Password: root (NOT ADVISED SECURITY SETTINGS!)
    ```
    Install then Execute installation.
    
![image](https://github.com/user-attachments/assets/8db039d6-2ff1-4336-ab0d-1ee5a0afca98)
  - Our step 6 requires us to run our **Internet Information Services** (IIS) as an **Administrator**, navigating to the PHP Manager in order to setup the correct file path.
      <h4>Search > IIS > PHP Manager > Register new PHP version > C:\PHP\php-cgi.exe</h4>
      
![image](https://github.com/user-attachments/assets/654e3cb8-042e-4415-ac44-d4b9c7648fe8)
  - Next, we will unzip our osTicket File located inside our osTicket-Installation-Files. Copy the upload folder, and navigate to the following:
    <h4>This PC > Windows (C:) > inetpub > wwwroot > Right Click and Paste</h4>
    Make sure to rename this **upload** folder to **osTicket** within the **wwwroot** file.
    
![image](https://github.com/user-attachments/assets/bd285aef-f557-40ec-8fdd-85ec90ea95a7)
  - For our step 8 we will begin by restarting our IIS Manager, reopening as admninistrator and navigating to the following:
    <h4>Sites > Default Web Site > osTicket > PHP Manager > Enable/Disable an Extension > Enable: php_imap.dll, php_intl.dll & php_opcache.dll</h4>

![image](https://github.com/user-attachments/assets/1ea7fc37-d972-471c-b664-e0867e132dfd)
  - On step 9, we will navigate to our **ost-sampleconfig.php** file and rename it to **ost-config.php**: 
    <h4>This PC > Windows (C:) > inpetpub > wwwroot > osTicket > include > ost-sampleconfig.php</h4>
    
![image](https://github.com/user-attachments/assets/374398dd-e69e-4335-b21b-e9876ff88f50)
  - Next, we will edit our osTicket permissions to Everyone:
    <h4>This PC > Windows (C:) > inpetpub > wwwroot > osTicket > include > ost-config.php > Properties > Security > Advanced > Disable Inheritance > Remove All > Add > Select a principal >           Everyone > Check Names + Ok</h4>
