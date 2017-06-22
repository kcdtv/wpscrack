# wpscrack
This is a copy of the original code from **Stefan Viehböck**  
The orignal dropbox download is down, the link was posted in Stefan's blog: https://sviehb.wordpress.com/2011/12/27/wi-fi-protected-setup-pin-brute-force-vulnerability/  
**wpscrack** was the first tool that performed WPS PIN brute force attacks.  
It was published the 29th of December 2011.  
It was developed in backtrack with an ar9170 chipset and does not support a lot of devcies.  
It was more conceived as a PoC than as a "final tool"  
All credits for the WPS PIN brute force vulnerability and wpscrack goes to **Stefan Viehböck** 

_Original readme file by **Stefan Viehböck**_

PoC implementation of a brute force attack against WPS - PIN External Registrar

My test environment was Backtrack 5R1 + an Atheros USB adapter.
I used a mac80211/carl9170 driver but any mac80211-based driver should be ok.

DEPENDENCIES:  
`PyCrypto`  
`Scapy (2.2.0)` (does not come with Backtrack)  

USAGE:  
`iwconfig mon0 channel X`  
`./wpscrack.py --iface mon0 --client 94:0c:6d:88:00:00 --bssid f4:ec:38:cf:00:00 --ssid testap -v`  

further usage:  
`./wpscrack.py --help`  

REFERENCES:  
http://sviehb.wordpress.com/2011/12/27/wi-fi-protected-setup-pin-brute-force-vulnerability/  
http://download.microsoft.com/download/a/f/7/af7777e5-7dcd-4800-8a0a-b18336565f5b/WCN-Netspec.doc  
http://hostap.epitest.fi/wpa_supplicant/
