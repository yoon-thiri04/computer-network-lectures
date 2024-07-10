## OSI Model

💡International Standard Organisation(`ISO`) is a multinational body dedicated to the world wide agreement on international standard.

💡The ISO standard that covers all aspects of the network communications is the **`Open System Interconnections (OSI)`** model

💡ISO is the organization, OSI is a model. OSI model is not a protocol, it is a model for understanding and designing a network architecture.

💡The OSI model is a layered framework for the design of network systems that allow communications between all types of computer system.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/3807d5bd-4c57-4cef-bb1b-3baebea437e3" alt="OSI model Layer" width="500" text-align="center" />


## Layered Architecture
### Layer-to-layer Communication
💻 Device A sends a message to the device B. (through intermediate nodes)

💻 At the sending site, the message is moved down from layer7 to layer1.

💻 At layer1, the entire package is converted to the form that can be transferred to the receiving site.

💻 At the receiving site, the message is moved up from layer1 to layer7.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/f490b78d-c6a4-4de1-8863-5cdeba44b3e9" alt="layer to layer architecture" width="500"/>

### Encapsulation
✏️ The process starts at layer7( the application layer) and then moves from layer to layer in descending, sequential order.

✏️ At each layer, a header can be added to the data unit. At layer2, a trailer may also be added and then pass through physical layer (layer1).

✏️ its destination, the signal passes into layer1 and each block of data reaches the next highter layer, the headers and trailers attached are removed.

<img src="https://github.com/yoon-thiri04/computer-network-lectures/assets/152978538/48937219-480f-4b29-9f20-d941e921c3a4" alt="Encapsulation" width=500/>



