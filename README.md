# Output of the security analysis of SDN-based-IoT-Oriented Blockchain Protected E-Voting System

This repository contains the experimental output of the voting system. It also contains the output of Scyther Tool for showing the security status of the voting system at different functional levels.

## Table of contents
- [I. Architecture of the SDN-based-IoT-Oriented Blockchain Protected E-Voting System](#i-architecture-of-the-sdn-based-iot-oriented-blockchain-protected-e-voting-system)
- [II. Output of authentication processes of booth and voter process.](#ii-output-of-authentication-processes-of-booth-and-voter-process)
- [III. Output of results of successful vote casting and counting of votes](#iii-output-of-results-of-successful-vote-casting-and-counting-of-votes)
- [IV. Demonstration of Programming level security](#iv-demonstration-of-programming-level-security)
- [V. Demonstration of Operating System level security](#v-demonstration-of-operating-system-level-security)
- [VI. Demonstration of Network level security](#vi-demonstration-of-network-level-security)

## I. Architecture of the SDN-based-IoT-Oriented Blockchain Protected E-Voting System

![Experimental Setup of the Voting System](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/e051704c-7d55-4ba7-8eab-87379e48435a)

Fig 1. Experimental Setup of the Voting System.

Fig 1 shows the test-bed setup of the multi-layered voting system. Three computers running Ubuntu 20.04 OS are used representing District Level, State Level and Country Level. One Raspberry Pi is also used to represent Booth Level. This Booth Level device is responsible for collecting votes from the valid voters.

## II. Output of authentication processes of booth and voter process.

![Successful Authentication of Booth](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/f2f4f048-1bfa-4696-a324-7e11a1b491cd)

Fig 2. Successful Authentication of Booth.

![Invalid Authentication of Booth](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/b527a68c-3e6f-486e-b7bf-8ce32d2d1933)

Fig 3. Invalid Authentication of Booth.

![Dsiplay of Voter Authentication](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/2c8a9bbe-d20b-47d1-82fe-c6cebe81d52c)

Fig 4. Display of Voter Authentication.

Fig 2 and Fig 3 show the successful and invalid authentication of Booth respectively. While communicating between the Booth device and the District machine, Booth information is encrypted using Elliptic Curve Cryptography (ECC). The booth details are already stored in the district blockchain and it is used to validate the device. Fig 4 represents the authentication of Voter. Voter information is also stored in district level blockchain and his/her voting status is also stored there.

## III. Output of results of successful vote casting and counting of votes

![Display of Vote Casting System](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/a81146a5-8216-4608-9aab-4ab7ca132f6f)

Fig 5. Display of Vote Casting System.

![Display of Counting of Votes](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/1b00b4dc-874b-4180-a11c-cb4b78b7130e)

Fig 6. Display of Counting of Votes

Fig 5 shows the casting of vote by a valid voter where the voter has to choose a desired candidate from a list of potential candidates. After choosing the candidate, the vote is saved and sent it to the higher heirarchical layers. After voting process has completed, at a specific date and time counting of votes take place. It is represented in Fig. 6.

## IV. Demonstration of Programming level security

![Scyther output of Booth Authentication](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/adbb429b-483c-4308-95d1-9547af5880c1)

Fig 7. Scyther Output of Booth Authentication

![Scyther output of Voter Authentication](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/b2301f1e-59ec-4e5d-9e9d-9c8e1ecd3e0f)

Fig 8. Scyther Output of Voter Authentication

![Scyther output of voting process](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/f59c6cba-5a54-4e0b-a1f6-669291b13a04)

Fig 9. Scyther Output of Voting Process

Scyther is a formal protocol verification tool to ensure better security of the system. It verifies the security status of the proposed protocol.

## V. Demonstration of Operating System level security

![NMAP_output](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/d94e7b19-b666-4835-b471-9147fdad5edc)

Fig 10. Output of NMAP commands

NMAP tool checks for any open ports and vulnerabilities available in the system.

## VI. Demonstration of Network level security

![Iprables rules](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/9191fe5d-9f80-44d6-b628-036578a645ef)

Fig 11. Output of Iptables rules

![Suricata output](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/03a04f6a-9e56-4db5-aa6a-2e66dda4c107)

Fig 12. Running of Suricata Tools

![Wireshark Output](https://github.com/Indrason/SDN-based-IoT-Oriented-Blockchain-based-E-Voting-System/assets/26199016/39e504ca-8e4a-4329-a37a-5e9f3c529465)

Fig 13. Running of Wireshark Tool

IPtables rules are the software-based firewall for the linux platform.
