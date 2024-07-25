# Bioinformatics Club
Welcome to our Bioinformatics Club's GitHub repository!

## About Us
The Bioinformatics Club is a community of researchers, students, and enthusiasts passionate about bioinformatics. 
It's a collaborative environment where members can learn, share knowledge, and work on projects that advance the field of bioinformatics.

More resources will be shared as we progress.

Happy learning!
## Before we begin
### Set up WSL on your windows computers and install ubuntu virtual machine from the microsoft store. If you're running a Linux platform...Awesome!!!

1. Open Windows Powershell as administrator( press Win + X then select "Windows PowerShell (Admin)" )
2. Check if wsl is enabled by running the following command:
```
   Get-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
 ```   
If WSL is enabled, you should see "State: Enabled" in the output

3. If not enabled you can enable it by running the following command:
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
4. Enable the Virtualization Machine Platform:
```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
Restart your computer for changes to effect

5. Set up Wsl-2 as your default after the restart by running:
```
wsl --set-default-version 2
```
6. Open Windows Microsoft Store and search for Ubuntu: Install version 24.04
7. Once installed, launch Ubuntu 24 from the Start menu (You can choose to pin it to task bar for quick access)
   When you launch it for the first time, you will be prompted to create a new user account and password.(create a password that's easy to remember)
8. In the terminal update the package lists and then upgrade the installed packages by running:
```
sudo apt update
```
```
sudo apt upgrade
```
9. Install a package manager, conda, by installing either the mamba or miniconda version to manage your packages and environments during analysis:
    
For Mamba:
```
wget https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Linux-x86_64.sh
```
   For Miniconda:
   ```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh .
```
   
10. Install the downloaded package:
```
bash Mambaforge-Linux-x86_64.sh
```
or
```
bash Miniconda3-latest-Linux-x86_64.sh
```
11. Restart your terminal after installation to reload configuration files:
```
$SHELL
```
or
```
. ~/.bashrc
```
This is a shorthand command of "source ~/.bashrc"

12. If successful you should see the name (base) displayed before your system name on the terminal
13. Configure channels to conda by adding them to the Condarc channel list:
```
conda config --add channels <channel-name>
```
Add the 'conda-forge' and 'bioconda' channels for now; in future you may need to configure more channels as you install different packages
14. You are now ready to tackle bfx challenges😎
    
