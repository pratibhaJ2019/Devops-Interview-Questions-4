# Devops-Interview-Questions
Devops Interview Questions

## Software Delivery
### What is Continuous Integration?
It is the part of software development strategies where fresh code commits are integrated and code is tested with the changes.Many of the developers are working on different part of coding of project. They may working on some functions which are later has to be integrated and tested accordingly. While this module is integrated with some of the branch,(respected to some branch ) it needs to be tested that they are working correctly with other modules of project. This integration has to be tested to make sure that this code modules works correctly with other module. The process of combining code modules with fresh changes to the main module is called as continuous Integration.It is very usefull for early bug discovery and bug fixes.By integrating regularly we can detect errors quickly and discovers them easily.

### What CI tools have you used?
As there are so many CI tools are available in market and each has their own advantages and limitations. The most popular CI tool nowdays and I have used is, jenkins. It is open source Integration Server that comes with numbers of plugins and huge community support.With the helps of plugins , its can able to provide many features. and with it's community support , we can find solution of any problem that we are facing while working with Jenkins.
### What is Continuous Delivery and why is it important?
Continuous Delivery is an extension to the Continuous Integration. It is a approach where teams ensure that the changes to the system are releasable. We achieve all these by ensuring that our code is always in deployable state.
We can achieve several benefits using continuous delivery. As follows,
##### Low risk releases :
This is the primary goal of continuous delivery is to be software deployments painless, low risk events, that can be performed at any time, on demand.
##### Faster Time to market
It is well known that traditional software development lifecycle take much time in Integration and Bug fixing.It make take weeks or even months to complete. When teams works together to automate the process of build and deployment, environment provisioning and so. by this way to cut off the time required for traditional SDLC process and speedup all the operations.

##### Higher Quality
When developers have automated tools that discovers regression in minute,  teams are freed to focus their effort on user research and higher level testing activities such as exploratory testing, usability testing, and performance and security testing.We can achieve this by building deployment pipeline.This activities are performed continously throughout the delivery process.This way we can ensure quality of product from beginning.
##### Lower costs.
By investing in build, test, deployment and environment automation, we substantially reduce the cost of making and delivering incremental changes to software by eliminating many of the fixed costs associated with the release process.
##### Better Products
Continuous delivery makes it economic to work in small batches. This means we can get feedback from users throughout the delivery lifecycle based on working software.
##### happier Teams
Software delivery teams can engage more actively with users, learn which ideas work and which don’t, and see first-hand the outcomes of the work they have done. By removing the low-value painful activities associated with software delivery, we can focus on what we care about most—continuously delighting our users.

## Linux
### How can you view running processes?
We can use ```top``` command for that. ```htop``` we can use for interactive process viewer.

### How do you check server uptime?
By using ```uptime``` command. by providing -p option, it will show the output in pretty format.

### How do you start/stop services?
To start or stop service , we can use service command with sudo option.
##### To start the services , we can use
```
sudo service <service-name> start
```
##### To stop the services, we can use
```
sudo service <service-name> stop
```

### How do you display the shell’s environment variables?
We can simply use ```printenv``` command for this.

### What does #!/bin/bash at the top of a script do?
The ```#!``` symbol call as Shebang. Shebang acts as an interpreter to execute the file(script file.).Like if we added #!/bin/bash then the interpreter shell here is bash shell. and all commands or the instructions specified in the script are executed by the bash shell.
### What does "&" after a command do?
Whenever we want to run the command or a script in background , then at last of command we use "&". It will use when some script or some command take much time for execution so that we don't need to wait for its execution or at the time when we don't want to loose shell prompt and want to continue with it.

### What does piping commands mean?
The piping ```|``` mean providing output of one command to the input to another command. Like if we want to check whether the particular user is available in the system we can first print the /etc/passwd file using ```cat``` and provide the output of this to ```grep``` to search the particular String in it. Like as follows
```
cat /etc/passwd | grep "sunrays"
```
The above command will result like
```
sunrays:x:1002:1002::/home/sunrays:
```
Otherwise it will be empty.

### What distributions have you used on servers?Why?
I have used Ubuntu and CentOS on servers. These are the mostly used distributions on cloud because of its Support , Ease of use, and Simplicity. These Distributions are open source and free to use. Both distributions has large community support and it's easy to learn.

## Configuration Management
### Which Configuration Management tools are you most comfortable with?
Ansible.

## Container
### How does Docker improve scalability, distributed computing, and efficiency vs. traditional cloud virtual machines?
With traditional cloud virtual machine, the speed of application deployment is somewhat slow as compared to docker because of following reasons.
##### 1. Traditional Cloud VM contains some of the unnecessary libraries and dependencies which makes them heavy.
##### 2. Because of this Heavy Libs/deps, the boot time is also more(In minutes).
##### 3. because of these unnecessary libs/deps , our resources are also wasted.(Like disk space, CPU, memory, N/W resources for some unncessary services and process.)
##### 4. Scale up any application is only possible with manual work or complicated script file.
Docker will overcome these all limitations and provides some challenging features like,
##### 1. Fast bootup time (In Seconds).
##### 2. Its does not contain any unnecessary libs/deps.(no wastage of resources)
##### 3. Mostly deal with quick application deployment.(With Dockerfile)
##### 4. We can use it with CICD pipeline.
Among these advantages, docker comes up with various inbuilt tools like docker-compose and docker swarm which makes multi-app container deployments possible. by using docker-compose , we can combine multiple app in the compose file , generally called docker-compose file, where we can specify our multiple apps and its interactions. Eg. MEAN stack Application.
By using docker swarm , the distributed application deployment is much easier. In swarm , we can connect multiple docker deamons by using overlay network and can deploy our app on these docker deamons using docker stack.
By using docker swarm mode, we can scale any application with a single command and able to create number of replicas of any application.
To scale our application in docker swarm mode , we simply use,
```
docker service scale <app-name>=<no-of-replicas>
```
