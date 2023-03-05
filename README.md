# vmwol
A script to wake up a vm with a magic packet under Linux with virsh.
It has to be run on the host.
It will listen on port 9 and once receiving a magic packet with the MAC Address of the VM it will launch the virsh command to wake it up. 

Replace <VM NAME> by the name of VM, and <VM MAC ADDRESS> with its MAC Address.

I made this script because most of the available script out there do not support passed through NIC as they are looking for the VM MAC Address by parsing the XML files of the VM.
