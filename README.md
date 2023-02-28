# Homelab practice labs

This repository contains the diagrams of all projects that I have made to learn about new technologies. I try to use open-source technologies to unlock the software's full potential and explore more features.

## Homelab 2021:

![diagram](./Homelab/2021/Home_Network-Primary_Slide.drawio.svg)

---

## HeadScale:

HeadScale is a dynamic VPN solution that allows peers to communicate with each other directly in a meshed topology to eliminate a single point of failure. [https://github.com/juanfont/headscale](https://github.com/juanfont/headscale)

This open-source technology allows end devices to communicate with each other in a meshed virtual private network topology.

### Diagram:

![diagram](./HeadScale-lab/HeadScale_Research_Project.drawio.svg)

### Lab screenshots:

This screenshot shows the clients approved to be a part of the meshed VPN network.

![image](https://user-images.githubusercontent.com/26883110/221480327-e8c12013-b953-473a-8241-6395cddb2542.png)

This screenshot shows the endpoints that client Debian-01 is connected to and the amount of traffic that has been passed over the VPN tunnels.

![image](https://user-images.githubusercontent.com/26883110/221480516-ddf5424d-a3b0-424e-8de0-20e176d04bd7.png)

This screenshots presents the interface of Pihole which is used for a DNS filtering and overriding DNS records.

![Picture](./HeadScale-lab/screenshots/Pi-Hole.png)

---

## NET year 2 capstone sandbox environment:

This diagram represents the sandbox environment I use to test technologies before deploying them into the production network of my capstone in NET year 2. Testing changes before deploying them allows me to confirm compatibility with the current setup. Sandbox testing reduces the amount of time I have to spend on troubleshooting.

In this diagram, there are 3 sites to demonstrate redundancy and high availability. The entire environment is virtualized in VMware workstation.

The following open-source solutions are used:

- NetBox: offline topology documentation system.
- PiHole: DNS filtering, and DNS resolver.
- Odoo: helpdesk internal ticking system.
- Pfsense: Acting as a firewall on each site and as a route on the ISP side (OSPF routing).

![diagram](./NET_Year_2_Sandbox_Environment/NET_Year2_Capstone_sandbox.drawio.svg)

---

## NET Classroom Lab Environment:

This diagram replaces all the small labs that work on top of each other in the first term of the second year of the NET program.

I have worked on all these labs with [Anil Mehrotra](https://www.linkedin.com/in/anil-mehrotra-4a5475266/).

Things we have learned:

- How to setup site to site Virtual Private Network (VPN) tunnels.
- How to capture traffic and analyze it with Wireshark.
- How to implement light weight Access Point (AP) through a wireless controller.
- How to implement an autonomous Access Point (AP).
- How to implement RADIUS for centralized authentication for the network equipment.
- How to implement a SIP based (open standard) Voice Over IP (VoIP) solution. This is the part for the phones.
- How to configure firewall rules.
- How to isolate guest network traffic from corporate network traffic.
- How to setup a VPN gateway on the edge of the network for remote (off site) users.

![diagram](./NET_Classroom_Lab_Environment/Classroom_Environment.drawio.svg)

---

## Pfsense OSPF over IPsec:

This lab got me to understand better how OSPF would work over an IPsec VPN tunnel. I use and prefer OSPF as a top preference when I am required to do routing in a lab environment.

![diagram](./Pfsense_OSPF_over_IPsec/OSPF_over_Hub-in-Spoke-IPsec_VTI_Pfsense.drawio.svg)

---

## Pfsense High Availability Dual WAN Active-Passive:

This lab has 2 firewalls demonstrating high availability without interruption in the event of a firewall failure.

![diagram](./Pfsense_HA_dual_WAN/Pfsense_HA_CARP-Page-1.drawio.svg)

---

## Pfsense Common Address Redundancy Protocol (CARP) with OSPF:

This lab is an implementation of CARP as a First Hop Redundancy Protocol (FHRP) alongside OSPF for dynamic routing updates.

![diagram](./Pfsense_CARP_With_OSPF/Pfsense_CARP_with_Single_Area_OSPF-Page-1.drawio.svg)

---

## Proxmox Hyper-converged Infrastructure (HCI) Cluster:

This lab is an implementation of three nodes of Proxmox in HCI mode. The Ceph protocol allows the three Proxmox nodes to act in HCI mode.

![diagram](./Proxmox_HCI_Cluster/Proxmox_HCI_Lab_exported.drawio.svg)