# bS-UnrealIRCd-Installer-Tutorial


```
Author: BlackLeakz
Version: 0.1
Website: https://blackzspace.de/

```


# This is a UnrealIRCd Setup/Installation Tutorial !!!
```
(FOR THE LAZY ONES)
There is a full automated setup script available if you dont want to learn how to do it by yourself, you can just run the script and follow the instructions on the screen.
```

# What is UnrealIRCd ?

```
UnrealIRCd is an popular Internet Relay Chat Server Software for setting up your very own IRC-Server.
```



# Step 1:

    ```
    [LINUX]

    Add a user for UnrealIRCd to your system like: "unrealircd"
    If you are using debian/ubuntu or something else run:
    
    root@linux:~$ useradd unrealircd

    Now look if the system has automatically added the home-dir to /home/unrealircd by using this command:

    root@linux:~$ ls -l /home

    If you see the folder is there, continue by loggin in to the user you created before and cd into the home dir!
    Else: Create the users home-folder by using this commands:

    root@linux:~$ mkdir /home/unrealircd && chmod 777 -R /home/unrealircd && chown unrealircd /home/unrealircd

    Now download the latest unrealircd version by using this command (make sure wget is installed):

    root@linux:~$ wget https://unrealircd.org/downloads/unrealircd-latest.tar.gz

    Now untar the archive!

    root@linux:~$ tar xvf *.gz

    Now cd into the untared folder and typein this command:

    root@linux:~$ ./Config

    Now you can defaultly always press Enter until its finished!
    Run now following command:

    root@linux:~$ make

    after compiling run:

    root@linux:~$ make install

    Now you can cd into the installation dir of unrealircd by using this commands:

    root@linux:~$ cd ..
    root@linux:~$ cd unrealircd

    You are finished by installing unrealircd, you can find the example config in unrealircd/conf/example.conf

    Copy this config to unrealircd/conf/unrealircd.conf and edit the conf as needed!"

    ```

