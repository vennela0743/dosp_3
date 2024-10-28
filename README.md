# dosp_3
# project : Chord Protocol Implementation in Pony


## Team Members
- Chandan Abhishek Muchukota
- Vennela Priya Penumuchu
## What is Working
 - The basic Chord protocol functionality is working. This includes network join, finding successors, and routing messages. Each peer actor can successfully join the Chord ring and maintain its finger table, allowing efficient lookup. The average hop count is being calculated as required, and all nodes are able to handle their allotted requests per second, with results being displayed upon completion.

## What is the largest network you managed to deal with

- The largest network tested successfully involved 10,000 peers and 100 requests per node. The system handled this load efficiently, maintaining stable routing performance with an average hop count that remained within expected limits for a distributed hash table setup. However, beyond this point, the network encountered noticeable delays and occasional resource limitations due to the increased overhead in message handling and finger table maintenance.

This performance threshold can vary based on hardware and available resources, but current tests confirm that the network remained efficient and stable up to 10,000 nodes.

