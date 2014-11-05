###Information

You need to download the plugin `check_vmware_snapshot.pl` from Simon at this link : 
[Download here!](https://labs.consol.de/nagios/check_vmware_snapshots/)

###Exemple

######Check snapshot count on all VMs
```
define host {
  use             snapshot-vmware
  host_name   		esx01.local
  address		      10.0.0.1
  _LOGIN	        esx_user
  _PASSWORD       Pa$$w0rd
  _BLACKL         --blacklist 'replica'
}
```
