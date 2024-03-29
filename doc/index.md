# Online Safety from Tasks and Tools

## Risk Assessment

I have taken a risk assessment model to attempt to Identify Tasks, Hazards, Control Measures, which should 
when matched with identified tool combinations provide the best protection for users

The risk assessment - [[Risk.odt]]

### Tasks

Each task should be equivelent to some general use case, the tasks will then identify the possible Hazards based of the type of communication and content.

### Hazards 

A hazard is a general group of threats based on the motivation/objective behind the threat.

| Hazard       | Description                                         | 
| ----         | ----                                                | 
| Tool Failure | Your computer hardware/software being exploited     | 
| Tool Theft   | Your computer being stolen                          | 
| Theft        | Theft of value                                      | 
| Surveillance | Spying                                              | 
| Infiltration | infiltration into the actual system/protocol        | 
| Manipulation | Manipulation of Objective                           | 
| Censorship   | Blocking of content travelling through the internet | 

### Information

Categories of information that a Hazard could compromise:

| Information Type | Description                                                                       |
| ----             | ----                                                                              |
| Personal         | Personal information about family, generally used for Identity theft or blackmail |
| Behavioural      | Used for Selling marketing and Spying                                             |
| Financial        | Used to denote things with monetary value                                         |
| Ideological      | Used to identify political affiliation                                            |
| Operational      | used to identify actions and resist pressure                                      |
| Private          | information of a sensitive nature                                                 |


### Likelihood 

In an environment with *no* protection the possibility of compromise.


### Control Measures 

Based on the Hazard and the Information threatened, define countermeasures to use to mitigate risk.

| #    | Control Measure                          | Description                                                                                 |
| ---- | ----                                     | ----                                                                                        |
| 1    | OS Choice                                | A Secure OS with minimal active exploits                                                    |
| 2    | Firewall                                 | Protect yourself by blocking direct attacks                                                 |
| 3    | Anti-virus/Malware                       | Ensure you have Updated and active virus/malware protection, this may be provided by the OS |
| 4    | Computer Use Training / User Competanccy | When using a computer to acieve tasks safely.                                               |
| 5    | Cache Purging                            | Ensure any processed information is not left where it can be recovered                      |
| 6    | Password Safe                            | If you have access passwords/keys, ensure they are stored in a safe location                |
| 7    | Disk Encryption                          | Protect your sensitive information from being recovered from silenced disks                 |
| 8    | Transport Encryption                     | Encrypt data during transit, must be to an acceptable* standard                             |
| 9    | Out of Band Authentication               | Authentication where a shared secret had been securely passed and verified                  |
| 10   | Authenticated Encryption                 | Encryption that has been secured by an Authenticated secret                                 |
| 11   | Transport Anonymity                      | A transport to prevent identification of actors communication                               |
| 12   | Perfect Forward Secrecy.                 | Encryption which ,even if intercepted, cannot be decrypted with any key                     |
| 13   | Anonymity                                | Communication cannot be identified or authenticated.                                        |
| 14   | Platform Selection                       | Choice of platform/network to use based on protection given (https://tosdr.org)             |
| 15   | Authentication                           | Authentication (less strong then OOB?)                                                      |
| 16   | System Use Training                      | A Specific system needs to give special usage information to the user                       |
| 17   | Communication Obfuscation                | Allowing communication to concealed                                                         |


(* If it is good enough for trade agreements.) 

## Tools

Tools available brief description and control measures implemented, I have just taken this from my limited uderstanding of these systems, and will need further investigation to be sure of these claims.
There are also grades of protection provided by packages, which isn't investigated here, but an implementation of some kind of grading may be useful but also difficult.

| Name                | info                                               | Description                                     | Implements     |
| ----                | ----                                               | ----                                            | ----           |
| GnuPG               | https://gnupg.org                                  | Public-Private Key Cryptography                 | 15, 10         |
| OTR                 | https://otr.cypherpunks.ca                         | Private communications over instant messaging   | 13, 12, 15, 10 |
| MixMaster           | https://sourceforge.net/projects/mixmaster         | Anonymous Remailer                              | 11, 13         |
| Mixminion           | https://mixminion.net                              | Anonymous Remailer                              | 11, 13         |
| Freenet             | https://freenetproject.org                         | Decentralised node driven encrypted network     | 8, 11, 13      |
| Gnunet              | https://gnunet.org                                 | Encrypted peer to peer Network                  | 11, 8          |
| I2P                 | https://geti2p.net                                 | Anonymous network layer                         | 11, 13         |
| tor                 | https://torproject.org                             | Decentralised Node driven Encrypted Network     |                |
| Namecoin            | http://namecoin.info                               | Anonymous registry                              |                |
| shred               | see apt                                            | Secure file deletion                            | 5              |
| tinc                | http://www.tinc-vpn.org                            | encrypted peer to peer network                  | 11             |
| zyre                | https://github.com                                 | Proximity based Peer to peer framework          |                |
| Retroshare          | https://retroshare.sourceforge.net                 | friend to friend secure decentralised net       |                |
| Briar               | https://briarproject.org                           | Proximity based encrypted peer to peer network  |                |
| Pond                | https://pond.imperialviolet.org                    | Forward secure async messaging (Experimental)   |                |
| cjdns               | http://cjdns.info                                  | Encrypted IPv6 with PPK for address allocation  |                |
| Mumble              | http://mumble.info                                 | Encrypted VoIP                                  |                |
| Jitsi               | https://jitsi.org                                  | Encrypted VoIP/Video with OTR plugin            |                |
| CCNx                | https://www.ccnx.org                               | Content Secured network with name addressing    |                |
| Tahoe-LAFS          | https://www.tahoe-lafs.org                         | Decentralized cloud storage system              |                |
| Blackadder          | https://www.fp7-pursuit.eu/PursuitWeb/?page_id=338 | information centric networking                  |                |
| Tribler             | https://www.tribler.org/                           | Peer to peer file sharing                       |                |
| Psyced              | http://www.psyced.org/                             | Encrypted distributed chat and messaging system |                |
| Bittorrent          | https://www.bittorrent.org/                        | Peer to peer file sharing                       |                |
| tox                 | https://tox.im/                                    | Distributed Encrypted VoIP/video Messaging      |                |
| linphone            | https://linphone.org                               | Distributed Encrypted VoIP/video Messaging      |                |
| MonkeySphere        | https://web.monkeysphere.info                      | Extending OpenPGP Web of trust                  |                |
| OpenVPN             | https://openvpn.net                                | Encrypted network tunnelling VPN                |                |
| vidalia             | https://www.torproject.org/projects/vidalia.html   | GUI Controller for tor software                 |                |
| Onioncat            | https://www.onioncat.org                           | An anonymous VPN adapter                        |                |
| https-everywhere    |                                                    | Force https usage in mozilla browser            |                |
| mozilla-noscript    |                                                    | Block javascript in mozilla browser             |                |
| mat                 | https://mat.boum.org                               | Metadata Anonymization tool                     |                |
| onionshare          |                                                    |                                                 |                |
| corkscrew           |                                                    |                                                 |                |
| torsocks            |                                                    | A SOCKS proxy for tor                           |                |
| obfsproxy           |                                                    |                                                 |                |
| obfs4proxy          |                                                    |                                                 |                |
| torbrowser-launcher |                                                    |                                                 |                |
| flashproxy          |                                                    |                                                 |                |
| iodine              |                                                    |                                                 |                |
| macchanger          |                                                    |                                                 |                |
| privoxy             |                                                    |                                                 |                |
| cryptsetup          |                                                    |                                                 |                |
| gnupg-agent         |                                                    | Persistance of GPG instance                     |                |
| kleopatra           |                                                    |                                                 |                |
| monkeysign          |                                                    | Leverage PGP's web of trust                     |                |
| parcimonie          |                                                    |                                                 |                |
| pinentry            |                                                    |                                                 |                |
| seahorse            |                                                    | Cryptographic key management                    |                |
| signing-party       |                                                    |                                                 |                |
| irssi-plugin-otr    |                                                    |                                                 |                |
| pidgin-otr          |                                                    |                                                 |                |
| ooniprobe           | https://ooni.torproject.org/                       | Internet censorship measurement tool            |                |
| pass                | see apt                                            | Store you passwords with gpg (command line)     |                |
| assword             | see apt                                            | Secure password management and retrieval        |                |
| haveged             |                                                    |                                                 |                |
| keepassx            |                                                    | Password safe                                   |                |
| msva-perl           |                                                    |                                                 |                |
| nautilus-wipe       |                                                    |                                                 |                |
| pwgen               |                                                    | generate secure passwords                       |                |
| secure-delete       |                                                    | secure data deletion                            |                |
| claws-mail-pgpmime  |                                                    | PGP mail client plugin                          |                |
|                     |                                                    |                                                 |                |

These are preliminary and there is a definite need to have thouruogh analysis of these tools bassed on their claims.

## Use Training
The Largest point of failure in all these systems is the user, through misconfiguration of misuse, we need a method to engage the user and their thought process when using these tools. from general computer use to using a specific tool, these should be easily accessible to the user and available from Context of use use, the language must be as clear as possibly and accessibly to users of all levels.


## Development
    
`blends-dev`
    Tools to build metapackages from template 

`git-buildpackage`
    build deb packages from metapackages,

Debian Live 
    For Building live images

## Examples
Ham Radio Example of build page:
http://blends.debian.org/hamradio


