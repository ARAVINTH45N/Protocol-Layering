# RTS of Protocol Layering

# Real-Time Protocol Layering Using Food Delivery System

## Introduction

Protocol layering is a communication architecture where communication is divided into multiple layers and each layer performs a specific function.

This project explains protocol layering using a real-time food delivery system scenario which is easy to understand and relatable to everyday life.

The project covers:
- Single Layer Protocol
- Three Layer Protocol
- Encapsulation
- Decapsulation
- TCP/IP Suite
- Real-time communication

---

# Single Layer Protocol

## Concept

Single layer protocol represents direct communication between two users without any intermediate processing layers.

---

# Real-Time Scenario

Two friends are sitting in a college canteen.

Aravinth directly tells his friend:

```text
"Order one chicken burger."
```

The friend listens and places the order directly.

Communication happens only through:
- Speaking
- Listening

This is a Single Layer Protocol

---

# Single Layer Architecture
<img width="1536" height="1024" alt="gen 1" src="https://github.com/user-attachments/assets/650acca2-8000-4e00-844e-6ac3af1ab4b0" />


---

# Working Process

1. Aravinth speaks directly.
2. Friend listens.
3. Friend places order.
4. Communication happens instantly.

---

# Advantages

- Very simple
- Fast communication
- No complex processing

---

# Disadvantages

- No security
- Works only for short distance
- No data protection

---

# Three Layer Protocol

<img width="1536" height="1024" alt="gen 3" src="https://github.com/user-attachments/assets/021ed606-6f80-46e2-b3b4-5563d72e6904" />
<img width="1536" height="1024" alt="gen 2" src="https://github.com/user-attachments/assets/a7f026b9-5a26-433d-a286-6e0abe8850a7" />




## Concept

In three layer protocol, communication is divided into multiple layers and each layer performs a different function.

---

# Real-Time Scenario

Aravinth is now at home and wants to order food using a food delivery application.

The communication happens through different layers.

---

# Layer 3 – Application Layer

The user selects:
- Food item
- Address
- Payment method

Example message:

```text
"Deliver one chicken burger to Hostel Block A"
```

This original readable message is called:

# Plaintext

---

# Layer 2 – Security Layer

The application encrypts:
- Address
- Payment details
- Mobile number

Example:

```text
Deliver Burger
↓
A7#K92@LM
```

Now the message becomes:

# Ciphertext

This provides:
- Security
- Privacy
- Safe communication

---

# Layer 1 – Delivery Layer

The encrypted order is:
- sent to server
- assigned to delivery partner
- routed using GPS
- delivered physically

This acts like:
# Send/Receive Layer

---

# Receiver Side Process

After delivery:

## Layer 1
Customer receives food.

## Layer 2
Application verifies payment and decrypts details.

## Layer 3
Customer sees original order details and confirmation.

This reverse process is called:

# Decapsulation

---

# Three Layer Architecture

![Three Layer Protocol](images/three_layer_food_delivery.png)

---

# Encapsulation and Decapsulation

## Encapsulation

Adding information layer by layer before transmission.

### Process

```text
Food Order
↓
Encryption
↓
Server Processing
↓
Delivery Assignment
↓
Transmission
```

---

## Decapsulation

Removing information layer by layer at receiver side.

### Process

```text
Delivery Received
↓
Verification
↓
Decryption
↓
Original Order Displayed
```

---

# Encapsulation and Decapsulation Diagram


<img width="1536" height="1024" alt="gen 3" src="https://github.com/user-attachments/assets/ef9653ac-d6e2-4a4b-9d86-ebb356248c45" />

---

# TCP/IP Suite Relation

The food delivery system can also be compared with the TCP/IP suite.

| Food Delivery System | TCP/IP Layer |
|---|---|
| Food Delivery App UI | Application Layer |
| Encryption & Security | Transport Layer |
| GPS Routing | Internet Layer |
| WiFi / Mobile Network | Network Access Layer |

---

# TCP/IP Suite Diagram

<img width="1536" height="1024" alt="gen 4" src="https://github.com/user-attachments/assets/75e71f56-318e-47bb-ae29-345d697a9080" />


---

# Comparison Between Single Layer and Three Layer Protocol

| Feature | Single Layer Protocol | Three Layer Protocol |
|---|---|---|
| Communication Type | Direct | Layered |
| Security | No | Yes |
| Complexity | Simple | Moderate |
| Distance Support | Small | Large |
| Encryption | No | Yes |
| Processing | Minimal | Multi-layer |

---

# Real-Time Applications

## Single Layer Protocol
- Face-to-face communication
- Classroom interaction
- Direct talking

## Three Layer Protocol
- Food delivery apps
- Online shopping
- Banking applications
- WhatsApp communication
- Secure transactions

---

# Cisco Packet Tracer Simulation

## Network Topology

```text
User PC ---- Switch ---- Server ---- Delivery System
```

---

# Simulation Objective

To simulate:
- food order request
- packet transfer
- layered communication
- encapsulation
- decapsulation

using Cisco Packet Tracer.

---

# Devices Used

| Device | Quantity |
|---|---|
| PC | 1 |
| Switch | 1 |
| Server | 1 |

---

# Simulation Steps

## Step 1
Add:
- PC
- Switch
- Server

## Step 2
Connect devices using:
- Copper Straight Through Cable

## Step 3
Assign IP addresses.

## Step 4
Enable HTTP service on server.

<img width="1918" height="1076" alt="image" src="https://github.com/user-attachments/assets/f387a520-3a69-458e-9c33-8be68d05c466" />


## Step 5
Use simulation mode.
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2e843a24-4634-4723-bca5-0a529006a36f" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5e5f4692-914b-4add-95c4-609198f9bc49" />

<img width="1919" height="1076" alt="image" src="https://github.com/user-attachments/assets/33278b4c-4262-4811-a42d-ec0de4eebf24" />


## Step 6
Observe packet transfer and layer communication.

---

# Expected Output

- Successful communication between user and server
- Packet movement through layers
- Encapsulation and decapsulation process
- Real-time protocol layering demonstration

---

# Conclusion

Protocol layering divides communication into multiple layers where each layer performs a dedicated function.

Using the food delivery system example makes protocol layering:
- easy to understand
- practical
- real-time relatable

Modern applications use layered communication for:
- security
- scalability
- reliability
- efficient data transfer

---

# Viva Questions

## 1. What is protocol layering?
Protocol layering is dividing communication into multiple functional layers.

## 2. What is a single layer protocol?
Direct communication using one layer.

## 3. What is plaintext?
Original readable message.

## 4. What is ciphertext?
Encrypted unreadable message.

## 5. What is encapsulation?
Adding information layer by layer during transmission.

## 6. What is decapsulation?
Removing information layer by layer at receiver side.

## 7. Why is encryption important?
To provide security and privacy.

## 8. Which protocol model is used in real networks?
TCP/IP Suite.

## 9. What is the role of the application layer?
Handles user interaction and communication.

## 10. Give a real-time example of protocol layering.
Food delivery applications.

---

# References

1. Data Communications and Networking – Behrouz A. Forouzan
2. Computer Networks – Andrew S. Tanenbaum
3. TCP/IP Protocol Suite Documentation
4. Cisco Networking Concepts

---

# Author

## Aravinth N
B.E Electronics and Communication Engineering  
Saveetha Engineering College
