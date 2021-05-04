This is multichannel sensor
each channel represent EIGRP neighbor status
and neighbors count in each AS

1. Copy file psPowerEIGRP.exe to \PRTG Network Monitor\Custom Sensors\EXEXML folder
2. Copy files EIGRPv2.ovl to \PRTG Network Monitor\lookups\custom folder
3. Go to PRTG->Setup->System Administration->Administrative Tools for the Core Server
 and click Load Lookups and File Lists
4. In devices settings add credentials for Linux/Solaris/Mac use SNMP v3 user as Linux user and auth and priv keys (must be same) as Linux password
5. Add EXE/Script Advanced sensor, in dropdown list, select psPowerEIGRP.exe
6.Parameners must be: -h %host -u %linuxuser -a sha -ap %linuxpassword -x aes -xp %linuxpassword