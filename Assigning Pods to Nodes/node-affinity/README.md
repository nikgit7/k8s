#Node Affinity


Node affinity is conceptually similar to nodeSelector, allowing you to constrain which nodes your Pod can be scheduled on based on node labels. 
There are two types of node affinity:

**requiredDuringSchedulingIgnoredDuringExecution:**  
The scheduler can't schedule the Pod unless the rule is met. This functions like nodeSelector, but with a more expressive syntax. This is also called Hard Scheduling.


**preferredDuringSchedulingIgnoredDuringExecution:**
The scheduler tries to find a node that meets the rule. If a matching node is not available, the scheduler still schedules the Pod. This is called Soft Scheduling.
