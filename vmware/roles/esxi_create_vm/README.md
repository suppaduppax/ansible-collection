Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
| variable | choices | description
| --- | --- | ---
vm_vcenter_managed  | &bull; True<br>&bull; **False** <- default |
vcenter_hostname | required |
vcenter_username | required |
vcenter_password | required |
datacenter | required |
validate_certs | &bull; yes<br>&bull; **no** ← default |
vm_vcenter_path | | Defaults to `<vcenter_datacenter>/<vm_folder>/vm`
vm_name | required |
vm_state | &bull; absent<br>&bull; poweredon<br>&bull; powered-on<br>&bull; poweredoff<br>&bull; powered-off<br>&bull; **present** ← Default<br>&bull; rebootguest<br>&bull; reboot-guest<br>&bull; restarted<br>&bull; suspended<br>&bull; shutdownguest<br>&bull; shutdown-guest |
vm_os | required |
esxi_hostname | required |
vm_disk_size_gb | | Defaults to 8 
vm_disk_type | &bull; thin<br>&bull; thick<br>&bull; eagerzeroedthick ← default |
vm_datastore | required |
vm_memory_mb | | Defaults to 2048)
vm_memory_reservation | &bull; True<br>&bull; **False** ← default |
vm_memory_reservation_mb | | Defaults to vm_memory_mb |
vm_num_cpus | | Defaults to 1 |
vm_scsi | &bull; buslogic<br>&bull; lsilogic- <br>&bull; lsilogicsas<br>&bull; **paravirtual** ← default |
vm_network | | Defaults to 'VM Network'|
vm_network_device | | Defaults to 'vmxnet3' |


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
