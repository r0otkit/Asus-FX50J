OS X/macOS on Asus FX50J(X/K Series)
====================================


This project targets at giving the relatively complete functional OS X for both Asus FX50JX and FX50JK. Before you start, there's a brief introduction of how to finish powering up OS X on your laptop:

1. Create a vanilla installation disk(removable disk).
2. Install Clover with UEFI only and UEFI64Drivers to the installation disk just created. 
3. Replace the origin Clover folder with the one under my Git/Asus-FX50J/CLOVER.
4. Install OS X.
5. Once you finish installation of OS X, you can do the following steps to finish the post installation of OS X.

How to use deploy.sh?
----------------

Download the latest version installation package/directory by entering the following command in a terminal window:

```sh
git clone https://github.com/syscl/M3800
```
This will download the whole installation directory to your current directory(./) and the next step is to change the permissions of the file (add +x) so that it can be run.


```sh
chmod +x ./M3800/deploy.sh
```


Run the script in a terminal windows by(Note: You should dump the ACPI tables by pressing F4/Fn+F4 under Clover first and then execute the following command lines):

```sh
cd Asus-FX50J
./deploy.sh
```

Reboot your OS X to see the change. If you have any problem about the script, try to run deploy in DEBUG mode by 
```sh
./deploy.sh -d
```

Note: For two finger scrolling you need to change the speed of the Scrolling once to get it work and also have to enable them in Trackpad preferences.

Change Log
----------------
2016-6-28

- First commit.