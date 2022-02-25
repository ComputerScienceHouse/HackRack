# airgap
Documentation for CSH's Airgap lab.

## Overview

#### Hardware
- [ ] What will we be working with here? 
- [ ] Cover RJ45 jacks in that room > https://www.amazon.com/NTW-NL-PBK10-RD-Locking-Blocker-Color/dp/B00KN1HS60/ref=sr_1_4?keywords=rj45%2Block&qid=1645752849&sr=8-4&th=1
- [ ] Locked or open rack? Depends on the level of trust and whether we want physical or virtual networking. If physical we should get NICs with >4 ports

#### Software
- [ ] Golden image on a container or proxmox level?
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

#### Vectors (ranked by priority high to low):
- [ ] Ethernet
- [ ] USB
- [ ] WiFi
- [ ] Bluetooth
- [ ] Other physical interfaces

#### User Experience
- [ ] We can't do SSO or standard homedirs, this should probably just be one username and password
- [ ] What level of access and trust on proxmox do users get?


Sources:
ESET Jumping the Air Gap - https://www.welivesecurity.com/wp-content/uploads/2021/12/eset_jumping_the_air_gap_wp.pdf
