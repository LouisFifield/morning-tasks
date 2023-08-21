# Load Balancing
​
Can you decide what type of load balancing from the notes might work best for the following situations;
​
- A chat service where users maintain active connections for a while
​
I think the least connection load balancing setup will be the most applicable for this application as new requests will be sent to the server with the fewest active connections. This means each new request gets the highest possible quality connection and all users get a similar level of quality service.

- An AI image generation API with paid tiers

People using different tiers are likely to have different usage requirements, with those on the paid tiers having higher usage. It will therefore be useful for this application to use weighted round robin load balancers. This is useful as requests with the highest loads are assigned to servers which have the capacity to handle more significant loads. 
​
- A social media website that has users all over the world
​
Source request information load balancers may be the most useful for this application as they use information identifying where the social media user is from in the world and then the load balancer connects them to a server in a region located closest to them, thus providing them with the lowest latency and best quality service specific to their location.

- An authorisation service that takes the same amount of time for each request

As each request takes the same amount of time, the round robin load balancing setup will be the most useful for the application as is distributes requests evenly in a sequential manner. 
​
- A gaming server that requires low latency

The least response time load balancers will be the most useful for this application as this system choses the server which takes the least time to respond.