# JavaScript running with Python in VSCode windows

If you are unable to find the `npm` command in the VS Code terminal, it means that Node.js and npm are not installed or not properly configured on your system.

To resolve this issue, you can follow these steps:

1.  Install Node.js: Visit the official Node.js website ([https://nodejs.org](https://nodejs.org/)) and download the latest version of Node.js for your operating system. Follow the installation instructions provided for your specific platform.
    
2.  Add Node.js to PATH: During the Node.js installation process, make sure to check the option that adds Node.js to your system's PATH environment variable. This will allow you to access the `npm` command globally from any terminal or command prompt.
    
3.  Verify the installation: After the installation is complete, open a new terminal in VS Code and run the following command to verify that Node.js and npm are installed:
    
    cssCopy code
    
    `node --version
    npm --version` 
    
    These commands should display the version numbers of Node.js and npm, respectively. If you see the version numbers, it means that Node.js and npm are installed correctly.
    
4.  Restart VS Code: If you installed Node.js and npm while VS Code was open, it's recommended to restart VS Code to ensure that it picks up the newly installed binaries.
    

Once you have successfully installed Node.js and npm, you should be able to use the `npm` command in the VS Code terminal without any issues.

**yarn : File C:\Users\(userID)\AppData\Roaming\npm\yarn.ps1 cannot be loaded because running scripts is disabled on this system.**

The error message you received indicates that running scripts is disabled on your system, which is preventing the execution of the `yarn` command. This is a security measure in place on some systems to prevent the execution of potentially harmful scripts.

To resolve this issue, you can modify the execution policy in PowerShell to allow running scripts. Follow these steps:

1.  Open PowerShell as an administrator: Right-click on the PowerShell icon and select "Run as administrator".
    
2.  Check the current execution policy: In the elevated PowerShell window, run the following command:
    
    `Get-ExecutionPolicy` 
    
    This command will display the current execution policy for PowerShell.
    
3.  Change the execution policy: To change the execution policy to allow running scripts, run the following command:
        
    `Set-ExecutionPolicy RemoteSigned` 
    
    This command sets the execution policy to "RemoteSigned" which allows the execution of scripts signed by a trusted publisher, but requires a digital signature for all other scripts.
    
4.  Confirm the change: When prompted to change the execution policy, type "Y" and press Enter to confirm the change.
    
5.  Close the PowerShell window: Once the execution policy is changed, you can close the elevated PowerShell window.
    
After following these steps, open a new terminal in VS Code and try running the `yarn` command again. It should now execute without the "running scripts is disabled" error.

**Now you can install the LayerZero Client**

![image](https://github.com/mrsheeda/blockchain/assets/59265997/87f7cab7-a996-47f3-b283-e74005bc0b14)
