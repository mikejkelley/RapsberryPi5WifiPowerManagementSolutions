The Raspberry Pi 5 has seemingly common Wifi reliability problems related to multiple, overlapping power management systems. Turning the power management settings off will often return Pi 5 Wifi to a reliably working state.

Save wifi-powermanagement-off.service to /etc/systemd/system/wifi-powermanagement-off.service.

Alternately, you can always create the file with 'sudo nano /etc/systemd/system/wifi-powermanagement-off.service' and then copy the contents of wifi-powermanagement-off.service into the file, save, and exit.

Command the following: 
'sudo systemctl enable wifi-powermanagement-off' 
'sudo systemctl start wifi-powermanagement-off' 

Save wifi-powersave-off.service to /etc/systemd/system/wifi-powersave-off.service

Issue the following commands:

'sudo systemctl daemon-reload'

'sudo systemctl enable wifi-powersave-off.service'

'sudo systemctl start wifi-powersave-off.service'

Your Pi 5 Wifi should now be returned to a reliably working state. 
