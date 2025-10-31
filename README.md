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
