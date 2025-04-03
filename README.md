# Educational Institute Network Design Using Cisco Packet Tracer

## Overview  
For this project, my team and I visited an Educational Institue, located in Islamabad, Pakistan, to study and mimic their network design. Based on our observations and requirements, we implemented a structured network that reflects their organizational setup.  

## Objectives  
- Create a functional network design that isolates departments for security while ensuring server accessibility for all.  
- Implement routing protocols (OSPF and EIGRP) to enable automatic route determination.  
- Design a network that mimics the real-world scenario of the Ministry of Education.  

## Network Implementation  

### VLAN Design  
To logically segment the network, we created five VLANs, each representing a department or function:  

- **VLAN 10 (Education):** Dedicated to the Education department.  
- **VLAN 20 (Professional-Training):** Handles professional training activities.  
- **VLAN 30 (International-Coordination):** Focuses on international coordination.  
- **VLAN 40 (Policy-Maker):** Reserved for policy-making activities.  
- **VLAN 50 (Server):** Contains servers accessible by all departments and vice versa.  

### VLAN Access Control  
- Departments (VLANs 10, 20, 30, and 40) were isolated from one another to ensure data privacy and enhance security.  
- VLAN 50 (Server) was configured to allow access from all departments while also having access to them.  

## Routing Protocols  
We used the following routing protocols to ensure dynamic and efficient routing:  

- **OSPF (Open Shortest Path First):** Administrative distance of 110.  
- **EIGRP (Enhanced Interior Gateway Routing Protocol):** Administrative distance of 90.  
- Routes between VLANs were determined automatically, prioritizing EIGRP due to its lower administrative distance.  

## Network Layers  
The network design incorporated a layered approach for scalability and performance:  

- **Core Layer:** High-speed backbone connecting all major components.  
- **Distribution Layer:** Provides inter-VLAN routing and policy enforcement.  
- **Access Layer:** Connects end-user devices within the VLANs.  

## Security  
Access Control Lists (ACLs) were implemented to enforce department isolation:  
- Traffic between VLANs 10, 20, 30, and 40 was denied.  
- Traffic to and from VLAN 50 (Server) was explicitly permitted.  

## Testing and Results  
- **Connectivity:** All devices within a VLAN could communicate without issues, while inter-VLAN communication was restricted according to the policy.  
- **Server Accessibility:** All departments successfully accessed the server, and the server communicated with all departments.  
- **Dynamic Routing:** Both OSPF and EIGRP functioned as expected, automatically determining routes based on administrative distances.  

---

📌 *This project demonstrates a real-world network design approach with a focus on security, efficiency, and scalability.*  

# ip Assignment
<img width="399" alt="image" src="https://github.com/user-attachments/assets/0b3f5791-168e-47ec-b856-0dc6356933d2" />

# Screenshot
<img width="565" alt="image" src="https://github.com/user-attachments/assets/acb2bdf5-6401-40c1-b1ee-663c63a6bc05" />

