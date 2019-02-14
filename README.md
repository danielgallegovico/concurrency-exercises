# Concurrent programming exercises 

## Exercise 1

Print all the possibilities that the next two processes compounded by three instructions each can be executed if both processes are executed at the same time:

[Process 1] => x = 2 * x
 * => LOAD R1, X
 * => MULT R1, #2
 * => STORE R1, X

[Process 2] => x = x + 1
 * => LOAD R2, X
 * => ADD R2, #1
 * => STORE R2, X


## Exercise 2

Implement the Lamport's bakery algorithm without using any atomic operation (e.g. locks, synchronized...)
 
**Lamport Algorithm** 
Lamport envisioned a bakery with a current Customering machine at its entrance so each customer is given a unique ticket.

Current Customers increase by one as customers enter the store. A global counter displays the ticket of the customer that is currently being served.

All other customers must wait in a queue until the baker finishes serving the current customer and the next ticket is displayed.

When the customer is done shopping and has disposed of his or her ticket, the clerk increments the ticket, allowing the next customer to be served.
 
That customer must draw another ticket from the current Customering machine in order to shop again.
 

## Exercise 3
Implement a cyclic barrier just using semaphores.


## Excersise 4 
Implement a read-write lock using semaphores.
