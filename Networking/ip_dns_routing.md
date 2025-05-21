# IP address
- Its basically a unique identifier assigned to every device on a network.
- Issued by Router.
- Can be configured by editing the router settings. a.k.a Static Assigninment

## Private IP and Public IP thing
- ### Private IP: Assigned by Router to the devices within the local environment. Say a Home Office or Lab.

- ### Public IP: Assigned by ISP. All devices in the local network share this public IP. They will have individual Local/Private IPs within that network.


# DNS: Stands for Domain Name System
- From a web browser POV, The easy to read website address needs to be assigned to a specific numeric IP address. This conversion is handled by DNS.

- DNS servers, either by ISP or publicly available ones such as cloudfare DNS or Google DNS (8.8.8.8) take up this task.

Can be configured to use a customer DNS setup in the system **/etc/resolv.conf** file as well as router.

## How its done?
- Open the /etc/resolv.conf file.
```
nameserver 8.8.8.8
``` 
This does it for google
```
nameserver 1.1.1.1
```
This is for cloudfare DNS.

If nothing is set, The system uses ISPs default DNS settings.
# Routing
Routing refers to where the packets go.

```
ip route show
```
This shows the defaut gateway and the device i.e. Network adapter that is being used for routing data packets from external network such as internet.

## Adding a route

```
sudo ip route add 10.10.10.12/24 via 192.168.1.1 dev eth0
```
This adds route 10.10.10.12 through the gateway 192.168.1.1 using the network adapter eth0. 

## Deleting a route
```
sudo ip route del 10.10.10.12/24
```
This delete a route from the system