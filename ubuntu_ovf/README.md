Dependencies

Install packer
Install ovftool

# enable GuestIpHack to allow packer to determine the vm IP address before vmtools are installed
esxcli system settings advanced set -o /Net/GuestIPHack -i 1
# open inbound VNC connections on the firewall
esxcli network firewall ruleset set -e true -r gdbserver


./packer.exe build -var-file variables.json ubuntu.json


https://nickcharlton.net/posts/using-packer-esxi-6.html
https://www.packer.io/docs/builders/vmware-iso.html


TODO:
https://www.packer.io/docs/provisioners/ansible.html
