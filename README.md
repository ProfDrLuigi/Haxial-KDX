# Haxial KDX Server / Client / Tracker

Here I will describe the installation on a Linux system. For Windows and Mac you can directly start over (to the Documentation.pdf) and no extra installations are necessary.

First clone the repo
        
    git clone https://github.com/profdrluigi/haxial-kdx

If you are on Linux set all Linux binaries to executable:
    
    chmod +x KDX\ Client/*.lexe
    chmod +x KDX\ Server/*.lexe
    chmod +x KDX\ Tracker/*.lexe

# Server:

#### Because the app is 32 Bit only first install the 32 Bit library in your 64 Bit system: ####
    sudo apt install libstdc++5:i386

#### Starting the server ####
    ./KDXServer.lexe
    
#### Doing initial setup ####
    KDX Server initial setup.  Press enter to continue.
    
    Creating new accounts file.  Enter login for your administrator account.
    > admin
    
    Enter password for your administrator account.
    Make it difficult to guess or crack (more than a single dictionary word and include symbols).
    > ************

    Type password again to confirm.
    > ************

    Connecting with no login or password (guest access) allowed? [y/n]
    > n

    Setup complete!
    23/04/12 01:01:05 PM [] KDX Server started on 10.0.0.1:10700, 192.168.178.21:10700, 192.168.122.1:10700, 172.17.0.1:10700
    
After the setup is done and the server running you can now config your file structure (starts in Bases/Default):    
    
    
    drwx------ 2 pi pi 4096 Apr 12 14:58 'Admin Dropbox [DB]'
    drwx------ 2 pi pi 4096 Apr 12 14:58 'Uploads [UL]'
    drwx------ 2 pi pi 4096 Apr 12 14:58 'Software'

If needed you can now symlink the "Default" folder to another place on your harddisk. For further Details of using DropBox and UL Folders have at look at Page 21 in the Documentation.pdf

# Client:
Because the app is 32 Bit only first install the 32 Bit library in your 64 Bit system: ####
    
    sudo apt install libx11-6:i386
