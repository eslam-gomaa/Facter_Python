# Facter - Python



A Python function that returns a `dict` of system information from the `facter` command, which is similar in usage to ***Puppet Facter***

* For a List of the facts –> "https://puppet.com/docs/facter/3.9/core_facts.html
* The `facter` command gets the vast majority of the facts but not all of it
* The code is compatible with ***Python 2 & 3***



## Installation

Is as simple as installing `facter`

```bash
yum -y install facter
# OR
apt-get -y install facter
```



## Usage & Examples



Just use the `facter()` function



* Get the entire facts (**dict**)

```python
facter()
# print(facter())
```



* Get specific `fact`

```python

facter()['uptime']
# 19 days
facter()['osfamily']
# Debian
facter()['os']['family']
# Debian

facter()['interfaces']
# bond0,cirename0,docker0,eth0,eth1,eth3,lo,virbr0,virbr0_nic,vnet0,vnet1,vnet2,vnet3,vnet4,vnet5,vnet6,vnet7
facter()['ipaddress']
# 192.168.0.14

facter()['memoryfree_mb']
# 241675.46
facter()['processors']['physicalcount']
# 2

facter()['partitions']
# {'sda1': {'uuid': 'b1668946-dce2-4dbe-9767-50e001aa8c9b', 'size': '27340800', 'mount': '/', 'filesystem': 'ext4'}, 'sda2': {'uuid': '31a10231-b5e8-4c5a-9c2e-6d771a8cd218', 'size': '999424', 'mount': '/boot', 'filesystem': 'ext2'}, 'sda3': {'size': '131072', 'label': 'config-2', 'filesystem': 'iso9660'}, 'sda4': {'uuid': '1b3a34d5-960a-400e-aead-8d8e70514fa6', 'size': '1532071936', 'mount': '/var/lib/libvirt/images', 'filesystem': 'ext4'}}
```





---



Thank you

[Eslam Gomaa](https://www.linkedin.com/in/eslam-gomaa)





