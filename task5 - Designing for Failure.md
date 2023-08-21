# Designing for failure

​
Identify the kinds of failure readiness described below, giving your reasoning;
​

- A system that switches to a new server when one fails
  ​
  This is failover. Which is when an IT device automatically switches to a back up when the main device fails.


- Adding replica databases with a master database

This is redunancy, as the replica databases will be used in the case if the master database fails.
​

- Having a 2-3 colleagues who have access to the master password

This is redunancy, as it stops there being a single point of failure, for example if one person had access to the master password and that one person was ill, the company could not be able to gain access to the systems.
​

- Performing health checks on a server

This is monitoring, as the server would be monitored and then every now and again health checks would be carried out to identify how well the server is performing.
​

- Spreading out user requests over multiple machines rather than just one powerful one

This is load balancing, as the requests are spread out across different servers in order to balance the distribution of the loads.
