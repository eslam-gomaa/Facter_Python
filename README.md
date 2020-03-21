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
facter()['osfamily']
facter()['os']['family']

facter()['interfaces']
facter()['ipaddress']

facter()['memoryfree_mb']
facter()['processors']['physicalcount']

facter()['partitions']
```







Thank you

[Eslam Gomaa](https://www.linkedin.com/in/eslam-gomaa)





