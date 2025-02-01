Laden Sie unsere ausgewählten pfsense-ISOs unter https://github.com/CloudSentralDotNet/iso_pfsense/releases herunter

oder verwenden Sie alternativ diese direkten Download-Links:      

* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.6.0/pfSense-CE-2.6.0-RELEASE-amd64.img
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.5.2/pfSense-CE-2.5.2-RELEASE-amd64.iso
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.4.4/pfSense-CE-2.4.4-RELEASE-amd64.img     
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.4.2/pfSense-CE-2.4.2-RELEASE-amd64.img  
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.3.5/pfSense-CE-2.3.5-RELEASE-amd64.img    


Stecken Sie ein neues USB-Laufwerk ein, aber mounten Sie es nicht.

Überprüfen Sie die Laufwerksbezeichnung, indem Sie „sudo lsblk“ in einer Konsole ausführen.

Führen Sie „sudo dd bs=4M if=/path/to/pfsense.iso of=/dev/sdX status=progress && sync“ aus.

Ersetzen Sie sdX durch die Bezeichnung Ihres USB-Laufwerks, z. B.: sdc (seien Sie hier sehr vorsichtig!).

Der Synchronisierungsteil ist wichtig, lassen Sie ihn nicht aus!

Nach Abschluss des dd-Befehls ist Ihr Laufwerk bereit.
