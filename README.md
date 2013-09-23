barber
A barber shop consists of a waiting room with n chairs and the barber room
containing the barber chair. If no customer arrives, barber goes to sleep.If a
customer arrives in the shop and all the chairs are occupied, then the customer
leaves the shop. If the barber is busy but the chairs are available, the
customer sits on the free chair. If barber is asleep the customer wakes him up.

here we can consider two semaphores
1. barber semaphore
2. customer semaphore

as a customer enters the shop, it sends a signal to the barber semaphore to wake
 him up.
 
 the barber can serve only one customer at a time so we can infer that the
customers are in the critical section.

they follow mutual exclusion i.e. while one customer is being served(executed)
no other customer can be served. also we can say that the customers are in
critical section.



BUSY WAIT:
let us consider that there is only one shop in the entire city. so all the
customers would wait for the availability of the chairs int the shop. for that
they repeatedly check for the chairs and keep waiting untill the chair is
available. this is known as busy waiting


SPIN LOCK:

 a spinlock is a lock which causes a thread trying to acquire it to simply wait
in a loop ("spin") while repeatedly checking if the lock is available.

