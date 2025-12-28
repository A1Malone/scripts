# How to install My Arr Stack

You will need to create a compose.yml and have docker run it. This should also work in GUI's like dockage, Portaioner, etc.

## Installation

Before you install you will need to edit the location for where you want the volumes 

```yml
volumes:
      - [insert file path here]/Prowlarr:/config
      - [insert file path here]/Media/:/media
```

You will need to change this and it should auto create if path is not already made.



##reminder
you will need to use something like PROTON VPN to get a wireguard file and upload it in the wireguard folder in the qbittorrent located here:

```bash
nano [insert file path here]/Qbittorrent/wireguard/wg0.conf 
```

and insert the wiregaurd settings it generated it may look like this:
*PLEASE NOTE THAT EACH WIREGUARD CONFIGURATION IS DIFFERENT AND YOU MAY GET SOMETHING DIFFERENT JUST COPY AND PAST IT TO THE LOCATION ABOVE*

[Interface]
# Key for arr stack
PrivateKey = [This is an example]
Address = [This is an example]
DNS = [This is an example]

[Peer]
PublicKey = [This is an example]
AllowedIPs = [This is an example]
Endpoint = [This is an example]
