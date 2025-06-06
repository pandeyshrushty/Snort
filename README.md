SNORT
main configuration of SNORT

sudo apt-get install snort -y

ip a s(to ens33)

ifconfig(for ip address)

 sudo ip link set ens33 promisc on

sudo apt update
sudo apt install vim -y

sudo vim /etc/snort/snort.conf

:q!(for exit of snort conf)

sudo snort -T -i ens33 -c /etc/snort/snort.conf
sudo vim /root/vimc

exit to vimc
:wq


