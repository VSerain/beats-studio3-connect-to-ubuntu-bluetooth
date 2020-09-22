# Connect Beats Studio 3 to Ubuntu (Bluetooth)
A simple tuto for connect Beats headphone to Ubuntu 19.10

## Why ?
I have beats studio 3 headphone but, I want connected to ubuntu, the headphone remain unconfigured status (See unconfigured.png)

## Steps

 1. Copy config file for avoid not being able to go back `sudo cp /etc/bluetooth/main.conf /etc/bluetooth/main.back`
 2. Open for edit the main.conf file `sudo vi /etc/bluetooth/main.conf`
 3. Replace the line `#ControllerMode = dual` by `ControllerMode = bredr`
 4. Save config file
 5. Restart bluetooth service `sudo /etc/init.d/bluetooth restart`
 6. Go to bluetooth params and connect on your headphone

Find through https://www.reddit.com/r/archlinux/comments/g4boam/beats_solo_3_bluetooth_headset_wont_pair/
