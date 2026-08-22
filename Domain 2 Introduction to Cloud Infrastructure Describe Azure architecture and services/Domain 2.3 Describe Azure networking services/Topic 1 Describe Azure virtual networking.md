# Describe Azure Virtual Networking

## Overview
Azure virtual networks (VNets) are an extension of your on-premises network in Azure. They let Azure resources such as virtual machines, web apps, and databases communicate with each other, with users on the internet, and with your on-premises client computers.

A VNet provides the networking foundation for Azure resources so they can connect securely and efficiently.

## Key networking capabilities

### 1. Isolation and segmentation
- Azure allows you to create multiple isolated virtual networks.
- When you create a VNet, you define a private IP address space using public or private IP ranges.
- This IP range exists only inside the virtual network and is not internet-routable.
- You can divide the address space into subnets and assign different parts of it to different resources.
- You can use Azure-provided name resolution or configure the VNet to use an internal or external DNS server.

### 2. Internet communication
- You can enable incoming internet connections by assigning a public IP address to an Azure resource.
- You can also place a resource behind a public load balancer so it can receive internet traffic.

### 3. Communicate between Azure resources
Azure resources can communicate securely with each other in two main ways:
- Through the same virtual network or connected virtual networks
- Through service endpoints, which connect Azure resources such as Azure SQL Database and Storage accounts to a VNet

This improves security and helps route traffic efficiently between services.

### 4. Communicate with on-premises resources
Azure virtual networks can connect your local environment to Azure so both networks act like one larger network. There are three common methods:
- Point-to-site VPN: a client computer connects securely to the Azure VNet over the internet
- Site-to-site VPN: your on-premises VPN device or gateway connects to the Azure VPN gateway in a VNet
- Azure ExpressRoute: a dedicated private connection to Azure that does not travel over the public internet

### 5. Route network traffic
By default, Azure routes traffic between subnets, connected virtual networks, on-premises networks, and the internet.

You can also control routing with:
- Route tables: define how traffic should be directed
- Border Gateway Protocol (BGP): shares on-premises routes to Azure virtual networks
- User-defined routes (UDR): control routing between subnets or virtual networks

### 6. Filter network traffic
Azure virtual networks can filter traffic by using:
- Network security groups (NSGs): define inbound and outbound rules based on source, destination, port, and protocol
- Network virtual appliances (NVAs): specialized virtual machines that perform security or WAN optimization functions

### 7. Connect virtual networks
You can connect virtual networks using virtual network peering.
- Peering allows two VNets to connect directly to each other
- Traffic stays private and travels over the Microsoft backbone network, not the public internet
- Peered networks can be in different regions, which allows global networking across Azure

## Public and private endpoints
- Public endpoint: has a public IP address and can be accessed from anywhere in the world
- Private endpoint: exists inside a VNet and has a private IP address from that VNet's address space

## Summary
Azure virtual networking is a key part of Azure architecture. It provides:
- isolation and segmentation
- internet communication
- secure communication between Azure resources
- connectivity to on-premises resources
- traffic routing and filtering
- connectivity between virtual networks

This makes Azure networking flexible, secure, and scalable for many different workloads.
