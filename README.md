# Docker-MERN
<h2>Why use Docker?</h2>
<ol>
<li/>Consistency Across Environments
<li/>Isolation
<li/>Portability
<li/>Lightweight
<li/>Version Control
<li/>Scalability
<li/>DevOps Integration
</ol>

<H2>Important Docker Components</H2>
    There are primarily four components of Docker:
<ul>
    <li/>Docker client and server 
    <li/>Docker image 
    <li/>Docker registry 
    <li/>Docker container
</ul>
<p><b>A Docker Conatiner is a runnable insatance of a Docker Image.<b> We can create multiple instances/ Containers from just one image.
<b>Docker Volume is a Persistent data storage mechanism.</b>
<b>Docker Network is a Communications Channel that enables different Docker Conatiners to talk/ communicate to each other or with the external world. It creates connectivity allowing containers to share information.</b>
<b>Docker Workflow</b> comprises of 1. Docker Client 2. Docker Host(Docker Daemon) 3. Docker Registry(Docker Hub).
<br/>
Creating own docker image starts from a Special File called <b>Docker File</b>. It's a set of some specific instructions and keywords telling Dcoker how to create an image of our application. The four layers of instructions: From, Pull, Run and CMD.
<ul>
<li/>FROM: creates a layer based on Ubuntu, and then we add files from the Docker repository to the base command of that base layer.
<li/>WORKDIR [Pull]: Adds files from your Docker repository
<li/>COPY [Run]: Builds your container
<li/>CMD: Specifies which command to run within the container
</ul>
</p>

<H2>Advanced Docker Components</H2>
<ul>
<li/> Docker compose 
<li/> Docker swamp </ul>