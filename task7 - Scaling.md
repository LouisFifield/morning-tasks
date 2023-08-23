# Scaling
​
In this exercise, you will be given a scenario where some kind of scaling will need to occur to meet demand.
Read through the scenario and give any pros and cons for **both vertical and horizontal** scaling that you can think of, giving examples as to how that specific feature of scaling would positively or negatively affect the infrastructure, the company, or the client.
​
For example;
​
Horizontal Scaling:
​
    Pro
        Cost: This type of scaling can be cheap on demand for short periods of time.
​
    Con
        Data Synchronisation; When dealing with this kind of scaling, it might be difficult to have consistent data across all instances to provide a consistent user experience.
​
Vertical Scaling
​
    Pros
        ...
​
    Cons
        ...
​
## Scenario
​
An e-commerce website experiences a sudden surge in traffic due to a flash sale event. The website needs to handle the increased load efficiently to ensure smooth user experience and prevent downtime.
​
Horizontal Scaling:
​
    Pro
        Cost: This type of scaling can be cheap on demand for short periods of time.

        Redunancy: If one instance fails others can continue to provide the servers.

        Scalability: There is no limit to the amount of instances that can be added and connected to work together. 
​
    Con
        Data Synchronisation; When dealing with this kind of scaling, it might be difficult to have consistent data across all instances to provide a consistent user experience.

        Higher Costs: Some applications will need to be reconfigured in order to work on the new system architecture, which will cost the developers time and money.
        
​
Vertical Scaling
​
    Pros
        Simplicity: All that is needed is to add cpu, memory or storage to an existing storage, which does not impact the architecture of the application. Also as there is only one instance, it makes the whole system more simple to manage.

        Resource Utilisation: Instances get used closer to their full capacity, so there is less wastage of computational power.

        Cost effective: for smaller loads it is cost effective, because you do not need to add any more instances.
​
    Cons
        Scalability: As only one instance is being utilised, there is a limit to how powerful one instance can become, i.e. there is limits to cpu, storage and memory. 

        Single point of failure: If there is only one instance, if this instance fails, the whole system will fail. 

        Downtime: When scaling the single instance, it must be turned off to add server resources. 



## Extension
​
What scaling decision would you choose and what steps do you think you might take to achieve the desired infrastructure?

For this application I believe the most suitable infrastructure would be horizontal scaling. As this is a sale the website will not be experiencing this level of activity on a regular basis. Therefore it would be useful to add more servers temporarily to support this short term surge in use. As money is being made via customers logging on and paying. It is essential that there is no down time in the service, for this purpose vertical scaling would not be suitable, as the servers must be shut down to and more computational power. 
​
## More...
​
If you finish with this one, give one of your mentors a message for another scenario to have a go at