## Harbor-Storage-Management

An application to manage a high-bay harbor storage place containing a single rack with a given number of storage places (slots) of different sizes. 
Packets of different size can be stored and retrieved later on from the storage place by a crane.

The high-bay harbor storage consists of a number of slots, that are identified by their size, position and load capacity (max. supported weight). 
The crane allows to pick up packets at the loading position, move to the position of a slot, store the packet in it or remove the packet from the slot and transport it to the loading position. 
The crane is controlled with simple primitives; motors can be started to move it up, down, forward, backward or can be stopped.

The crane control simplifies the usage of the crane. The control class enables the harbor storage management to store a packet at a defined slot position including picking it up at the loading position and storing it in the rack without controlling the motors of the crane directly. 
Packets can not be rotated to fit in a slot. The control class also allows retrieving a packet from a defined position and transporting it back to the loading position.

The harbor storage management determines and manages where (in which slot) each packet is stored and allows to find stored packets by their description. The storage management offers methods which provide the functionality to store a packet dependent on the size and the weight of the packet.
Packets might be too big or too heavy for certain slots in the rack; thus, the management finds a suitable slot. 
Furthermore, the storage management offers the service to retrieve a packet later using its description.

A user interface was implemented to allow users to control the behavior of the harbor storage management.
