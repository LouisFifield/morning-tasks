# Docker
​
1. What is containerization, and how does it differ from virtualization?

Virtualisation make it possible to run multiple computers with multiple different operating systems on the hardware of a single physical server. Each computer or instance is called a virtual machine and its complete own OS. 

Containerisation is a lightweight form of virtualization which alllows you to package an applicationa nd its dependancies into a single unit called a container. This container includes everything the application needs to run, such as code, libraries and runtime environments. They run on the same operating system, as such they use less resources because they can use the same OS, where as Virtualisation uses more resources because they each have their own OS. Virtual machines are more isolated than containers, which means each VM cannot interact with each other, this provides security benefits. Whereas containers are all on a single operating system. In terms of portability, containers are highly portable because they include everything needed to run an application, and they run consistently across different environments. Virtualisation on the other hand is not so portable as they contain the whole operating system.

2. Why is containerization important in modern software development and deployment?

Containerisation is important in modern software deployment because applications rely on a number of dependancies, i.e. for a node application you will need to install, NPM, and other dependancies specific to the functionality of the app. Containerisation allows all of these dependancies to be placed in a single location, of which an image can be created and deployed elsewhere at speed and scale.
​
If your computer can run the container, it can run whatever is inside, i.e. As long as I have docker, I can run whatever is in the container. 

3. What is the difference between an image and a container in Docker?

Docker containers are the environments which execute the application code. Whereas a docker image is an executeable package that contains the necessary code, libraries, dependancies and configurations needed to run a specific application. They are typically built from a set of instructions defined in a Dockerfile, which specifies how to create the image. 
​
4. Can you give an example of a situation where you might choose to use Docker containers in a software development project?

If you wanted to create a Node application, you would create a docker file which would include all of the dependencies needed for that code.
​
5.If you were tasked with explaining Docker to someone who has never heard of it before, how would you describe it in a few sentences?

Docker is a technology which allows containers to be built on virtual machines. The technology can build, run and manage container, as well as deploy applications. 
​
## Extension
​
Fill in this cheat sheet throughout the day to help and remind you understand how to use Docker commands
​
| Command | Description |
| :-----: | ----------- |
|   ps    |
| images  |
|  pull   |
|  build  |
|   run   |
|  stop   |
​
| Flag | Description  
|:------:|---------------------------------------------------
| -a |
| -d |
| -t |
| -p |
​
Below is an example of a how you might format a docker command. (In documentation having something wrapped in square brackets [] denotes that it is optional to provide this in the command)
​
```bash
docker run [OPTIONS] <IMAGE[:TAG|@DIGEST]> [COMMAND] [ARG...]
```