### Ansible Playbook for adding host definition to Icinga

### Assumption: 
2. A working setup of [Icinga on Debian 7](https://wiki.icinga.org/display/howtos/Setting+up+Icinga+with+IDOUtils+on+Debian#SettingupIcingawithIDOUtilsonDebian-debmonInstall)
1. cfg_dir=/etc/icinga/servers in /etc/icinga.cfg

### Use

`ansible-playbook icinga-add-host.yml -vv --extra-vars="fqdn=FQDN_OF_THE_CLIENT address=IP_OF_THE_CLIENT"`

### TODO

Better handling of fqdn and ip address facts via hostvars
