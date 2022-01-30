Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
variable | choices | description
—|—|—
vm_vcenter_managed  | - True/- False <- default |
vcenter_hostname | required |
vcenter_username | required |
vcenter_password | required |
datacenter | required |
validate_certs | yes\no <- default |
vm_vcenter_path | | defaults to <vcenter_datacenter>/<vm_folder>/vm
vm_name | required |
vm_state | poweredon |
vm_os | required |
esxi_hostname | required |
vm_disk_size_gb | 8 |
vm_disk_type | - thin\-thick\-eagerzeroedthick <- default |
vm_datastore | required |
vm_memory_mb | default(2048) |
vm_memory_reservation | - True\- False <- default |
vm_memory_reservation_mb | | Defaults to vm_memory_mb |
vm_num_cpus | integer\1 <- default |
vm_scsi | 	- buslogic\- lsilogic- \lsilogicsas\- paravirtual <- default |
vm_network | VM Network <- default |
vm_network_device | vmxnet3 <- default |


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
