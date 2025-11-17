# Jarkom-Modul-4-2025-K40

## VLSM - GNS 3

### Topology

<img width="1781" height="848" alt="Screenshot 2025-11-15 094024" src="https://github.com/user-attachments/assets/115b8af1-0333-4cb7-a3da-1ff3a0ada9df" />

### VLSM

| Subnet       | Prefix | Required Hosts | Network ID     | Netmask         | Broadcast       | Range IP                  |
|-------------|--------|----------------|----------------|----------------|----------------|---------------------------|
| Mirdain     | /22    | 628            | 192.231.0.0    | 255.255.252.0  | 192.231.3.255  | 192.231.0.1 - 192.231.3.254 |
| Silmarils   | /23    | 381            | 192.231.4.0    | 255.255.254.0  | 192.231.5.255  | 192.231.4.1 - 192.231.5.254 |
| Balrog      | /23    | 256            | 192.231.6.0    | 255.255.254.0  | 192.231.7.255  | 192.231.6.1 - 192.231.7.254 |
| Beacon      | /23    | 279            | 192.231.8.0    | 255.255.254.0  | 192.231.9.255  | 192.231.8.1 - 192.231.9.254 |
| Khazad      | /24    | 252            | 192.231.10.0   | 255.255.255.0  | 192.231.10.255 | 192.231.10.1 - 192.231.10.254 |
| Melkor      | /24    | 250            | 192.231.11.0   | 255.255.255.0  | 192.231.11.255 | 192.231.11.1 - 192.231.11.254 |
| Arthedain   | /24    | 246            | 192.231.12.0   | 255.255.255.0  | 192.231.12.255 | 192.231.12.1 - 192.231.12.254 |
| Lindon      | /24    | 132            | 192.231.13.0   | 255.255.255.0  | 192.231.13.255 | 192.231.13.1 - 192.231.13.254 |
| Thrandull   | /24    | 129            | 192.231.14.0   | 255.255.255.0  | 192.231.14.255 | 192.231.14.1 - 192.231.14.254 |
| Morgul      | /25    | 102              | 192.231.15.0   | 255.255.255.128| 192.231.15.127 | 192.231.15.1 - 192.231.15.126 |
| Shadow      | /25    | 99             | 192.231.15.128 | 255.255.255.128| 192.231.15.255 | 192.231.15.129 - 192.231.15.254 |
| Gothmog     | /25    | 84             | 192.231.16.0   | 255.255.255.128| 192.231.16.127 | 192.231.16.1 - 192.231.16.126 |
| Edhil       | /25    | 73             | 192.231.16.128 | 255.255.255.128| 192.231.16.255 | 192.231.16.129 - 192.231.16.254 |
| Anarion     | /25    | 67             | 192.231.17.0   | 255.255.255.128| 192.231.17.127 | 192.231.17.1 - 192.231.17.126 |
| Palantir    | /26    | 46             | 192.231.17.128 | 255.255.255.192| 192.231.17.191 | 192.231.17.129 - 192.231.17.190 |
| Elrond      | /26    | 34             | 192.231.17.192 | 255.255.255.192| 192.231.17.255 | 192.231.17.193 - 192.231.17.254 |
| Imrahil     | /27    | 27             | 192.231.18.0   | 255.255.255.224| 192.231.18.31  | 192.231.18.1 - 192.231.18.30 |
| Erendis     | /27    | 27             | 192.231.18.32  | 255.255.255.224| 192.231.18.63  | 192.231.18.33 - 192.231.18.62 |
| Mirkwood    | /27    | 30             | 192.231.18.64  | 255.255.255.224| 192.231.18.95  | 192.231.18.65 - 192.231.18.94 |
| Doriath     | /27    | 17             | 192.231.18.96  | 255.255.255.224| 192.231.18.127 | 192.231.18.97 - 192.231.18.126 |
| Arnor       | /28    | 10             | 192.231.18.128 | 255.255.255.240| 192.231.18.143 | 192.231.18.129 - 192.231.18.142 |
| IronCrown   | /29    | 5              | 192.231.18.144 | 255.255.255.248| 192.231.18.151 | 192.231.18.145 - 192.231.18.150 |
| Hobbiton    | /29    | 4              | 192.231.18.152 | 255.255.255.248| 192.231.18.159 | 192.231.18.153 - 192.231.18.158 |
| Grond       | /29    | 4              | 192.231.18.160 | 255.255.255.248| 192.231.18.167 | 192.231.18.161 - 192.231.18.166 |
| Gwaith      | /29    | 4              | 192.231.18.168 | 255.255.255.248| 192.231.18.175 | 192.231.18.169 - 192.231.18.174 |
| Erebor      | /30    | 2              | 192.231.18.176 | 255.255.255.252| 192.231.18.179 | 192.231.18.177 - 192.231.18.178 |
| Utumno      | /30    | 2              | 192.231.18.180 | 255.255.255.252| 192.231.18.183 | 192.231.18.181 - 192.231.18.182 |

### Tree

<img width="1920" height="1080" alt="Add a little bit of body text (2)" src="https://github.com/user-attachments/assets/f30942fd-ff69-49c7-b510-9abc6e22b8ba" />

### Config

- Mirdain
```
auto eth0
iface eth0 inet static
    address 192.231.0.2
    netmask 255.255.252.0
    gateway 192.231.0.1
    dns-nameservers 192.168.122.1
```

- Silmarils
```
auto eth0
iface eth0 inet static
    address 192.231.4.2
    netmask 255.255.254.0
    gateway 192.231.4.1
    dns-nameservers 192.168.122.1
```

- Balrog
```
auto eth0
iface eth0 inet static
    address 192.231.6.2
    netmask 255.255.254.0
    gateway 192.231.6.1
    dns-nameservers 192.168.122.1
```
- Beacon
```
auto eth0
iface eth0 inet static
    address 192.231.8.2
    netmask 255.255.254.0
    gateway 192.231.8.1
    dns-nameservers 192.168.122.1
```
- Khazad
```
auto eth0
iface eth0 inet static
    address 192.231.10.2
    netmask 255.255.255.0
    gateway 192.231.10.1
    dns-nameservers 192.168.122.1
```
- Melkor
```
auto eth0
iface eth0 inet static
    address 192.231.11.2
    netmask 255.255.255.0
    gateway 192.231.11.1
    dns-nameservers 192.168.122.1
```
- Arthedain
```
auto eth0
iface eth0 inet static
    address 192.231.12.2
    netmask 255.255.255.0
    gateway 192.231.12.1
    dns-nameservers 192.168.122.1

```
- Lindon
```
auto eth0
iface eth0 inet static
    address 192.231.13.2
    netmask 255.255.255.0
    gateway 192.231.13.1
    dns-nameservers 192.168.122.1

```
- Thrandull
```
auto eth0
iface eth0 inet static
    address 192.231.14.2
    netmask 255.255.255.0
    gateway 192.231.14.1
    dns-nameservers 192.168.122.1

```
- Morgul
```
auto eth0
iface eth0 inet static
    address 192.231.15.2
    netmask 255.255.255.128
    gateway 192.231.15.1
    dns-nameservers 192.168.122.1
```
- Shadow
```
auto eth0
iface eth0 inet static
    address 192.231.15.130
    netmask 255.255.255.128
    gateway 192.231.15.129
    dns-nameservers 192.168.122.1
```
- Gothmog
```
auto eth0
iface eth0 inet static
    address 192.231.16.2
    netmask 255.255.255.128
    gateway 192.231.16.1
    dns-nameservers 192.168.122.1
```
- Edhil
```
auto eth0
iface eth0 inet static
    address 192.231.16.130
    netmask 255.255.255.128
    gateway 192.231.16.129
    dns-nameservers 192.168.122.1
```
- Anarion
```
auto eth0
iface eth0 inet static
    address 192.231.17.2
    netmask 255.255.255.128
    gateway 192.231.17.1
    dns-nameservers 192.168.122.1
```
- Palantir
```
auto eth0
iface eth0 inet static
    address 192.231.17.130
    netmask 255.255.255.192
    gateway 192.231.17.129
    dns-nameservers 192.168.122.1
```
- Elrond
```
auto eth0
iface eth0 inet static
    address 192.231.17.194
    netmask 255.255.255.192
    gateway 192.231.17.193
    dns-nameservers 192.168.122.1
```
- Imrahil
```
auto eth0
iface eth0 inet static
    address 192.231.18.2
    netmask 255.255.255.224
    gateway 192.231.18.1
    dns-nameservers 192.168.122.1
```
- Erendis
```
auto eth0
iface eth0 inet static
    address 192.231.18.2
    netmask 255.255.255.224
    gateway 192.231.18.1
    dns-nameservers 192.168.122.1
```
- Mirkwood
```
auto eth0
iface eth0 inet static
    address 192.231.18.66
    netmask 255.255.255.224
    gateway 192.231.18.65
    dns-nameservers 192.168.122.1
```
- Doriath
```
auto eth0
iface eth0 inet static
    address 192.231.18.98
    netmask 255.255.255.224
    gateway 192.231.18.97
    dns-nameservers 192.168.122.1
```
- Arnor
```
auto eth0
iface eth0 inet static
    address 192.231.18.130
    netmask 255.255.255.240
    gateway 192.231.18.129
    dns-nameservers 192.168.122.1
```
- IronCrown
```
auto eth0
iface eth0 inet static
    address 192.231.18.146
    netmask 255.255.255.248
    gateway 192.231.18.145
    dns-nameservers 192.168.122.1
```
- Hobbiton
```
auto eth0
iface eth0 inet static
    address 192.231.18.154
    netmask 255.255.255.248
    gateway 192.231.18.153
    dns-nameservers 192.168.122.1
```
- Grond
```
auto eth0
iface eth0 inet static
    address 192.231.18.162
    netmask 255.255.255.248
    gateway 192.231.18.161
    dns-nameservers 192.168.122.1
```
- Gwaith
```
auto eth0
iface eth0 inet static
    address 192.231.18.170
    netmask 255.255.255.248
    gateway 192.231.18.169
    dns-nameservers 192.168.122.1
```
- Erebor
```
auto eth0
iface eth0 inet static
    address 192.231.18.178
    netmask 255.255.255.252
    gateway 192.231.18.177
    dns-nameservers 192.168.122.1

```
- Utumno
```
auto eth0
iface eth0 inet static
    address 192.231.18.182
    netmask 255.255.255.252
    gateway 192.231.18.181
    dns-nameservers 192.168.122.1
```

## CIDR - Cisco Packet Tracer

### Topology

<img width="1402" height="616" alt="image" src="https://github.com/user-attachments/assets/777ae8a6-6314-4086-a8c8-d070f718ae23" />

### Pembagian IP - CIDR

| Subnet | Network ID | Netmask | Broadcast | Range IP |
|---|---|---|---|---|
| Mirdain | 192.231.0.0 | 255.255.252.0 | 192.231.3.255 | 192.231.0.1 - 192.231.3.254 |
| Silmarils | 192.231.4.0 | 255.255.254.0 | 192.231.5.255 | 192.231.4.1 - 192.231.5.254 |
| Balrog | 192.231.6.0 | 255.255.254.0 | 192.231.7.255 | 192.231.6.1 - 192.231.7.254 |
| Beacon | 192.231.8.0 | 255.255.254.0 | 192.231.9.255 | 192.231.8.1 - 192.231.9.254 |
| Khazad | 192.231.10.0 | 255.255.255.0 | 192.231.10.255 | 192.231.10.1 - 192.231.10.254 |
| Melkor | 192.231.11.0 | 255.255.255.0 | 192.231.11.255 | 192.231.11.1 - 192.231.11.254 |
| Arthedain | 192.231.12.0 | 255.255.255.0 | 192.231.12.255 | 192.231.12.1 - 192.231.12.254 |
| Lindon | 192.231.13.0 | 255.255.255.0 | 192.231.13.255 | 192.231.13.1 - 192.231.13.254 |
| Thrandull | 192.231.14.0 | 255.255.255.0 | 192.231.14.255 | 192.231.14.1 - 192.231.14.254 |
| Morgul | 192.231.15.0 | 255.255.255.128 | 192.231.15.127 | 192.231.15.1 - 192.231.15.126 |
| Shadow | 192.231.15.128 | 255.255.255.128 | 192.231.15.255 | 192.231.15.129 - 192.231.15.254 |
| Gothmog | 192.231.16.0 | 255.255.255.128 | 192.231.16.127 | 192.231.16.1 - 192.231.16.126 |
| Edhil | 192.231.16.128 | 255.255.255.128 | 192.231.16.255 | 192.231.16.129 - 192.231.16.254 |
| Anarion | 192.231.17.0 | 255.255.255.128 | 192.231.17.127 | 192.231.17.1 - 192.231.17.126 |
| Palantir | 192.231.17.128 | 255.255.255.192 | 192.231.17.191 | 192.231.17.129 - 192.231.17.190 |
| Elrond | 192.231.17.192 | 255.255.255.192 | 192.231.17.255 | 192.231.17.193 - 192.231.17.254 |
| Imrahil | 192.231.18.0 | 255.255.255.224 | 192.231.18.31 | 192.231.18.1 - 192.231.18.30 |
| Erendis | 192.231.18.32 | 255.255.255.224 | 192.231.18.63 | 192.231.18.33 - 192.231.18.62 |
| Mirkwood | 192.231.18.64 | 255.255.255.224 | 192.231.18.95 | 192.231.18.65 - 192.231.18.94 |
| Doriath | 192.231.18.96 | 255.255.255.224 | 192.231.18.127 | 192.231.18.97 - 192.231.18.126 |
| Arnor | 192.231.18.128 | 255.255.255.240 | 192.231.18.143 | 192.231.18.129 - 192.231.18.142 |
| IronCrown | 192.231.18.144 | 255.255.255.248 | 192.231.18.151 | 192.231.18.145 - 192.231.18.150 |
| Hobbiton | 192.231.18.152 | 255.255.255.248 | 192.231.18.159 | 192.231.18.153 - 192.231.18.158 |
| Grond | 192.231.18.160 | 255.255.255.248 | 192.231.18.167 | 192.231.18.161 - 192.231.18.166 |
| Gwaith | 192.231.18.168 | 255.255.255.248 | 192.231.18.175 | 192.231.18.169 - 192.231.18.174 |
| Erebor | 192.231.18.176 | 255.255.255.252 | 192.231.18.179 | 192.231.18.177 - 192.231.18.178 |
| Utumno | 192.231.18.180 | 255.255.255.252 | 192.231.18.183 | 192.231.18.181 - 192.231.18.182 |
| Fornost ↔ Amonsul | 192.231.18.184 | 255.255.255.252 | 192.231.18.187 | 192.231.18.185 - 192.231.18.186 |
| Amonsul ↔ Minastir | 192.231.18.188 | 255.255.255.252 | 192.231.18.191 | 192.231.18.189 - 192.231.18.190 |
| Amonsul ↔ Eregion | 192.231.18.192 | 255.255.255.252 | 192.231.18.195 | 192.231.18.193 - 192.231.18.194 |
| Minastir ↔ Anor | 192.231.18.196 | 255.255.255.252 | 192.231.18.199 | 192.231.18.197 - 192.231.18.198 |
| Minastir ↔ Amroth | 192.231.18.200 | 255.255.255.252 | 192.231.18.203 | 192.231.18.201 - 192.231.18.202 |
| Eregion ↔ Numenor | 192.231.18.204 | 255.255.255.252 | 192.231.18.207 | 192.231.18.205 - 192.231.18.206 |
| Numenor ↔ Gudur | 192.231.18.208 | 255.255.255.252 | 192.231.18.211 | 192.231.18.209 - 192.231.18.210 |
| Numenor ↔ Mordor | 192.231.18.212 | 255.255.255.252 | 192.231.18.215 | 192.231.18.213 - 192.231.18.214 |
| Mordor ↔ Erain | 192.231.18.216 | 255.255.255.252 | 192.231.18.219 | 192.231.18.217 - 192.231.18.218 |

### Penggabungan - CIDR

<img width="721" height="181" alt="image" src="https://github.com/user-attachments/assets/ca804660-4151-427c-aa9c-8de067b2f85c" />

<img width="728" height="182" alt="image" src="https://github.com/user-attachments/assets/590f5f5f-2dc4-4c1d-b59a-b9daccf409ff" />

<img width="727" height="106" alt="image" src="https://github.com/user-attachments/assets/f60ed6ad-81b1-40fa-a6c2-415a328deb5f" />

<img width="731" height="129" alt="image" src="https://github.com/user-attachments/assets/5f3d3368-d9dd-4f98-af85-e03330d153c3" />

<img width="726" height="148" alt="image" src="https://github.com/user-attachments/assets/082fc580-e1ca-433a-a80a-b52017c211ad" />

<img width="558" height="124" alt="image" src="https://github.com/user-attachments/assets/74cd40e9-984a-49bf-9dbe-a2cef805029a" />

<img width="553" height="178" alt="image" src="https://github.com/user-attachments/assets/17eaf69c-87cb-4ae1-9f86-f5c452a092be" />

<img width="551" height="118" alt="image" src="https://github.com/user-attachments/assets/bdb94779-e680-45b5-8fdd-abb19cb6f8c0" />

<img width="551" height="121" alt="image" src="https://github.com/user-attachments/assets/48a79fe3-eb7a-4433-ad4c-d2bdb43f3ffa" />






