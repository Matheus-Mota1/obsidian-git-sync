# Definition
Node is a struct that has primitive values and a one of those values is a [[pointer]] to the next Node creating a chain of nodes. The information will never be lost because one refers to the next 

---> Head --->  Node --->  Node ---> ...

To know the end of the node the first one will pointer to **NULL**. Also known as 0x0
address of memory

# Free 

We have to be careful freeing the pointer because it make us unable access the next node that the node points, so instead we have to create a new temporary pointer to be able to free the memory allocated to use the struct and still have access to the chain.


