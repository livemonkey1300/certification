# certification

Certification Note Personal


# Google Disk 
## Persisten disk 
- Attached via network 
- Survive VM terminate
- Bootable can attach VM on boot
- can be set to incremental backup
- can be scale 
- performance directly by scale 
- can be resize and can be set to read only 
- zonal and regional mode 
- - pd-standard 
- - pd-ssd
- - pd-balance
- - pd-extreme (zonal) configure for high end database iop can be config 
- Encrytion key support 
    - google manage 
    - customer provided 
    - customer managed

## Local SSD 
- More iop 
- directly attached to the vm 
- default size 375 GB up to 24 can be attached 
- data survice reset not stop or terminated
- cannot be re attached to differnet vm 

## Ram disk 
- tmpfs
- faster than local disk slower than memory 

### Max Number of persitend disk that can be attached 
- 16 on shared-core 
- 128 on other instance 

# Cloud Engine
## Notes

Use metadata to work , have a startup script and end script 
commonly used to gater instance metadata and migrate instance 
can alos be use to snapshot data and put it on a diffrent vm 

## Snapshot disk

not visible in s3 bucket 
is incremental 
doesn't run on local ssd only cloud storage
manage by snapshot services
can be schedualed.

Disk cannot be shrink in the cloud



# Google cloud core - Identity - IAM

Main role orginazation admin has allo roles
project creator roles witch allow to create role over project can be applied to org level 

the responsablity of the og admin are 
define iam policy 
determine the structure of the hierachy 
delegate rources per team an individual 
org admin don't have permission over folder and resource they have to assigne it to themself

folder can be use to segregate project 
cannot use iam to create user and group


IAM policy deny pass before allowed policies
google cloud sync can sync with ldap resourced and policies 