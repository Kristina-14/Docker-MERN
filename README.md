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
<p>
<h2>Docker Compose</h2>
Docker Compose is a tool for defining and running multi-container applications. It is the key to unlocking a streamlined and efficient development and deployment experience.

Compose simplifies the control of your entire application stack, making it easy to manage services, networks, and volumes in a single, comprehensible YAML configuration file. Then, with a single command, you create and start all the services from your configuration file.

Compose works in all environments; production, staging, development, testing, as well as CI workflows. It also has commands for managing the whole lifecycle of your application:</p>
<ul>
<li/>    Start, stop, and rebuild services
<li/>    View the status of running services
<li/>    Stream the log output of running services
<li/>    Run a one-off command on a service
</ul>
<h2>Docker Compose Watch</h2>
<p>Use watch to automatically update and preview your running Compose services as you edit and save your code.

For many projects, this allows for a hands-off development workflow once Compose is running, as services automatically update themselves when you save your work.
It allows to:
<ul>
<li/>    Sync
<li/>    Rebuild
<li/>    Sync-restart
</ul>

"watch" adheres to the following file path rules:
<ul>
<li/>    All paths are relative to the project directory
<li/>    Directories are watched recursively
<li/>    Glob patterns aren't supported
<li/>    Rules from .dockerignore apply
<ol>
<li/>    Use ignore to defined additional paths to be ignored (same syntax)
<li/>    Temporary/backup files for common IDEs (Vim, Emacs, JetBrains, & more) are ignored automatically
<li/>    .git directories are ignored automatically</ol>
</ul>
You don't need to switch on watch for all services in a Compose project. In some instances, only part of the project, for example the Javascript frontend, might be suitable for automatic updates.</p>
<h2>Docker Scout</h2>
<p>
Container images consist of layers and software packages, which are susceptible to vulnerabilities. These vulnerabilities can compromise the security of containers and applications.

Docker Scout is a solution for proactively enhancing your software supply chain security. By analyzing your images, Docker Scout compiles an inventory of components, also known as a Software Bill of Materials (SBOM). The SBOM is matched against a continuously updated vulnerability database to pinpoint security weaknesses. <b>Simply go to the Docker Scout section in the Docker Engine and select the application which we want to check.<b>

Docker Scout is a standalone service and platform that you can interact with using Docker Desktop, Docker Hub, the Docker CLI, and the Docker Scout Dashboard. Docker Scout also facilitates integrations with third-party systems, such as container registries and CI platforms.
</p>