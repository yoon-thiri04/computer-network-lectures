## OSI Model

💡International Standard Organisation(`ISO`) is a multinational body dedicated to the world wide agreement on international standard.

💡The ISO standard that covers all aspects of the network communications is the **`Open System Interconnections (OSI)`** model

💡ISO is the organization, OSI is a model. OSI model is not a protocol, it is a model for understanding and designing a network architecture.

💡The OSI model is a layered framework for the design of network systems that allow communications between all types of computer system.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/3807d5bd-4c57-4cef-bb1b-3baebea437e3" alt="OSI model Layer" width="500" text-align="center" />

---
## Layered Architecture
### Layer-to-layer Communication
💻 Device A sends a message to the device B. (through intermediate nodes)

💻 At the sending site, the message is moved down from layer7 to layer1.

💻 At layer1, the entire package is converted to the form that can be transferred to the receiving site.

💻 At the receiving site, the message is moved up from layer1 to layer7.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/f490b78d-c6a4-4de1-8863-5cdeba44b3e9" alt="layer to layer architecture" width="500"/>

---
### Encapsulation
✏️ The process starts at layer7( the application layer) and then moves from layer to layer in descending, sequential order.

✏️ At each layer, a header can be added to the data unit. At layer2, a trailer may also be added and then pass through physical layer (layer1).

✏️ its destination, the signal passes into layer1 and each block of data reaches the next highter layer, the headers and trailers attached are removed.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/48937219-480f-4b29-9f20-d941e921c3a4" alt="Encapsulation" width=500/>

---
## Physical Layer

☎️ To carry a bit stream over a physical medium. It deals with the mechanical and electrical specifications between interface and transmission media. Physical
layer is moving individual bit from one node to the next.

☎️ Physical layer is also concerned with the following:

   - 🥤**Physcical characteristics of interfaces and media:** It defines the characteristics of the interface between devices and the transmission media.
   - 🥤**Representation of bits:** It data contains a stream of bits (0s or 1s) with no interpetation. To be transmitted, bits must be encoded into signals (electrical or optical).
   - 🥤**Data rate:** The transmission rate (the number of bits sent each second).
   - 🥤**Synchronization of bits:** The sender and receiver must not use the same bit rate but must be synchronized at the bit level.
   - 🥤**Line Configuration:** It concerned with the connection of devices to a media. In a point to point configuration, two devices are connected through a dedicated link. In a multipoint configuration, a link is shared between several devices.
   - 🥤**Physical Topology:** It defines the connection of devices to a network. Devices can be connected using a mesh 🖥️ topology, a star⭐ topology, a ring💍 topology, a bus🚌 topology.
   - 🥤**Transmission mode:** It also defines the direction of transmission between two devices, simplex, half-duplex, full-duplex.
      - 👤 In simplex mode, only one device can send a message and the other can only receive ( a one-way communication➡️)
      - 👥 In half-duplex mode, two devices can send and receive but not at the same time.🔃
      - 👥 In full-duplex mode, two devices can send and receive at the same time.🔄

### Type of Topologies 
![network](https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/cb236376-89ef-4b79-abbe-598a24527565)

---
## Data Link Layer

🔗 The data link layer transforms the physical layer to a reliable link, it makes error free to the upper layer (Network layer). 

🔗 Other responsibilities of the data link layer include the following:

   - 🥦 **Framing:** It divides the stream of bits received form the network layer into frames.
   - 🥦 **Physical Addressing:** If the frames are to be distributed to on the network, add a header to the frame to determine the sender and/or receiver of the
frame. If the frame is intented for a system outside the sender network, the reciever address is the address of the connect the networok layer to the next one.
