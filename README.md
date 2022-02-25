# airgap & netlab
Documentation for CSH's Airgap and networking labs.

## Overview

#### Hardware
- [ ] Have 1 full height rack and several switches already in the project room. Will probably wait for the new stuff before speccing out hardware for the lab. 
- [ ] Topology for networking lab:
  - [ ] Will want a vm set up on one of the netlab machines that can manage the switches/routers
  - [ ] Several routers and switches (as many as we can fit)
  - [ ] We probably don't need that many physical machines, if the new ones are as powerful as I expect, but we will want beefy (many port) network cards so netlab computers can give VM's physical interfaces. Would also be cool to have some kind of patch panel so that NIC ports can be accessible from the front of the lab easily

#### Software
- [ ] Deepfreeze type solution on os level on all machines. Images will also be on all machines. 
  - [ ]  Types of images
    - [ ]  Clean windows
    - [ ]  Clean linux
    - [ ]  Clean MacOS
    - [ ]  Kali images
    - [ ]  Other images with different types of tooling? What other workloads would be useful here?
- [ ] What applications do we want and how do we handle their management?
  - [ ]  Internal/local package repo, or should we try to pre-install a lot of stuff. I think the former might be less resource intensive on individual VMS
- [ ] Pre-made environments with many systems for CTF pentesting???

## Security Considerations

#### Physical security

- [ ] Airgap lab will have these on machines https://www.amazon.com/NTW-NL-PBK10-RD-Locking-Blocker-Color/dp/B00KN1HS60/ref=sr_1_4?keywords=rj45%2Block&qid=1645752849&sr=8-4&th=1
- [ ] USB will be disabled in BIOS and firmware, but will also put lockouts on them. 

#### Vectors (ranked by priority high to low):
- [ ] Ethernet
- [ ] USB
- [ ] WiFi
- [ ] Bluetooth
- [ ] Other physical interfaces

#### User Experience
- [ ] We can't do SSO or standard homedirs, this should probably just be one username and password
- [ ] What level of access and trust on proxmox do users get?

# Networking lab

Sources:
ESET Jumping the Air Gap - https://www.welivesecurity.com/wp-content/uploads/2021/12/eset_jumping_the_air_gap_wp.pdf
