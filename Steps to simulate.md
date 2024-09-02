## Networks -

There are totally 4 networks.

**Network 1** – LAN 1

**Network 2** – LAN 2

**Network 3** – LAN 3

**Network 4** – LAN 4 + LAN 5 + LAN 6 + LAN 7

## Devices -

**LAN 1** - 2 PCs, 2 Servers, 1 Switch

**LAN 2** - 3 PCs, 2 Laptops, 1 Switch

**LAN 3, LAN 4, LAN 5, LAN 6, LAN 7** - 5 PCs, 1 Switch

## Cables –

**Between endpoint devices such as laptops, PCs and servers and switches** – Copper straight through

**Between switches** – copper cross over

**Between switch and router** – Copper straight through

## Additional modules –

![image](https://github.com/user-attachments/assets/e9fbb39f-4096-4c1a-ad97-25ccecb5b416)

The router initially could support only 2 fast-ethernet interfaces. When we add more than 2, then it gives error.

![image](https://github.com/user-attachments/assets/43a5ae48-5ef5-48ab-915f-2aa95fcd755b)

Hence, we add a NM-2FE2W Module. It provides two Fast-Ethernet interfaces for use with copper media, in addition to two Wan Interface Card expansion slots.
(We need to switch off the router before adding the module)

![image](https://github.com/user-attachments/assets/ba1e6438-3306-4cb2-885b-0b9b026347e6)

![image](https://github.com/user-attachments/assets/7e6444f9-96fd-4152-84a0-320b62e3d4c1)

Now, we can connect 4 fast-ethernet ports connecting the router and the 4 switches in 4 networks.

## How to configure? –

### Configuring endpoints IP address –

![image](https://github.com/user-attachments/assets/998f2552-74ba-451b-9a44-683b9e9c1389)

Click on the endpoint device to be configured.

Go to config → Interface → FastEthernet0

Enter the IP address. The subnet mask is configured automatically.

### Configuring endpoints Default gateway –

![image](https://github.com/user-attachments/assets/afc212f4-a2d0-4e03-bdff-55dd8436e4da)

Click on the endpoint device to be configured.

Go to config → Global → Settings

Enter the default gateway. (The interface of the router for that particular network)

### Identifying the interface –

![image](https://github.com/user-attachments/assets/08c7eb7a-c139-4596-9bb4-b4c3f6a724d5)

By hovering on the cable connecting router and the switch of a network, we can identify the interface of the FastEthernet.

We enter the default gateway of the network to that interface on the router.

### Configuring router –

![image](https://github.com/user-attachments/assets/21b85730-0889-4ced-a4cd-1391a19bf8e4)

Click on the router.

Go to config → Interface → FastEthernet0/0

Enter the IP address for the interface connecting the router and the particular network.

Turn on the interface.

## Configurations –

I am going to use Class C Public IP range - 192.0.0.0 to 223.255.255.0

### Network 1 –

![image](https://github.com/user-attachments/assets/5b5068e0-dc8f-427b-b9c1-dbd34c07fc7b)

### Network 2 -

![image](https://github.com/user-attachments/assets/76e5e809-29d5-43ca-99a2-a34adf8c7f7e)

### Network 3 -

![image](https://github.com/user-attachments/assets/a8d039c3-8397-4697-b880-78ec1b1d6977)

### Network 4 -

![image](https://github.com/user-attachments/assets/55d53d4d-52ac-4d43-aa77-d2ca99d0e6c0)

### Router - 

![image](https://github.com/user-attachments/assets/85e506b6-1dc6-4178-9aa7-bda799917179)

## Simulated Network - 

![image](https://github.com/user-attachments/assets/2b894df3-95c9-4427-99eb-20c6c6e2554c)

## Testing the connections –

![image](https://github.com/user-attachments/assets/bc525278-3c78-4e0e-a87d-d6a27c8ce7b8)

Click on the Simple PDU packet on the toolbar.
Click the source and destination devices of the packet.
The results whether the packet successfully reached its destination or failed can be viewed at the PDU list window at the bottom of the screen.

![image](https://github.com/user-attachments/assets/ae09d240-a41d-4789-b986-811ee842b40a)
