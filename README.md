# distributed-systems-notes


**what is a distributed system?**\
It can be defined as a collection of indepedent computers that appears a single coherent system to its users whenrein all systems/nodes are work togther to achieve a goal & they communicate by passing messages

### Terminologies

***A program***\
is the code you write.\
***A process***\
is what you get when you run it.\
***A message***\
is used to communicate between processes.\
***A packet***\
is a fragment of a message that might travel on a wire.\
***A protocol***\
is a formal description of message formats and the rules that two processes must
follow in order to exchange those messages.\
***A network***\
is the infrastructure that links computers, workstations, terminals, servers, etc. It
consists of routers which are connected by communication links.\
***A component***\
can be a process or any piece of hardware required to run a process, support
communications between processes, store data, etc.
***A distributed system***\
is an application that executes a collection of protocols to coordinate the actions
of multiple processes on a network, such that all components cooperate together
to perform a single or small set of related tasks.

### CHARACTERISTICS OF A DISTRIBUTED SYSTEM.

***Fault-Tolerant:*** It can recover from component failures without performing
incorrect actions.

***Highly Available:*** It can restore operations, permitting it to resume providing
services even when some components have failed.

***Recoverable:*** Failed components can restart themselves and rejoin the system,
after the cause of failure has been repaired.

***Consistent:*** The system can coordinate actions by multiple components often in
the presence of concurrency and failure. This underlies the ability of a distributed
system to act like a non-distributed system.

***Scalable:*** It can operate correctly even as some aspect of the system is scaled to a
larger size. For example, we might increase the size of the network on which the
system is running. This increases the frequency of network outages and could
degrade a "non-scalable" system. Similarly, we might increase the number of
users or servers, or overall load on the system. In a scalable system, this should
not have a significant effect.

***Predictable Performance:*** The ability to provide desired responsiveness in a timely
manner.

***Secure:*** The system authenticates access to data and services

### Main Challange while designing a distributed system?
*lack of global time
clocks, it's very hard to timestamp events is different processes and
order them globally*
