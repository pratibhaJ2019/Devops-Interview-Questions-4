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

## Source Control
### What types of source control programs are you comfortable with?
I'm comfortable with Git, which most popular, open source , Highly Secured , reliable, Distributed Source Control (VCS, Version Control System) System.
### What are the benefits of using source control?
To keep track of each an every change in the source code, we need Source Code Management System. Not only this,SCM will offer various feature for software development teams.
While in Software development, we need to keep track of each an every activity of code. Because many of the developers need to contribute in the single product development. Below some of the issue developer facing if there is not an SCM.<br>
<b>1. Where to submit changes</b><br>
More often developers need a single place to commit/submit their code. While in software development , lots of lines of code has to be submitted and merged to the main branch of software developemnt. Due to this all developers need the single place to submit /commit their code frequently.<br>
<b>2. Collaboration among teams</b><br>
Many of the developers in software development are working different parts of software, side-by-side. While sometimes they need to comunicate between each other for some kind of functionality in the software. At that time collaboration between the developers is very important. Also there are so many others teams are working on different part of software like testing or QA teams. Thus the collaboration between the teams is much important.<br>
<b>3. Frequent commits </b><br>
As we know that its not possible and suitable to complete some large task at one shot, developers will cut such tasks in small units and then start working on such units. Once this units are developed developers will need to commit this unit frequently. To handle such Frequent commit and code changes SCM is much important.<br>
<b>4. Reverting changes</b><br>
As the development goes on , at some point it is possibly happen that, some buggy code is commited to the main branch of software , due to which software will goes into the buggy state. Such cases , we need to revert back to the state where our software is free from that buggy code. Thus reverting back into the state where everything is working fine as expected is much important.<br>
<b>5. Adding new Feature in Software</b><br>
While in agile methodology , where we deliver software as a part of features , we need to work on each feature while the software development grows.In such cases , adding the new feature code in the main branch is not a good way. for such situation, we need to create new branch for such feature and when we sure that the feature development is complete and working as expected , we need to add/merge this new feature branch to our main software branch.<br>
<b>6. And so on </b><br>
To efficiently solve such issues and provides effective communication, collaboration, speed to the development teams, we need SCM.

### Describe some branching strategies that you have used?
Whenever we want to add some feature in the software , instead of adding that feature code to the main branch of software, It is better idea to create new branch for that feature and add all that feature related code to that newly created branch only. By using this way , we can easily separate the business logic for that particular feature. Once that feature development is done and we sure that this feature can now merged to the main branch of software, then we simply merge that branch to the master.

### Give an example of a good commit message?
The good commit message gives the following answers efficiently.<br>
<b>WHY(The Need, may be bugfix,feature addition,performance,stabilty,realiability or just a change)</b><br>
<b>HOW(The address to the issue)</b><br>
<b>WHAT(The effects on the software)</b><br>
Example as follows:
Consider we are going to add offers feature to the git , and we are going to create new branch for it and added the first page for that.<br>
<br> -----------------------------------------------------------<br>
Created layout file and Java file for hot offers.<br>
AndroidProjects/E-comExpress/offers/main/offers.java <br>
AndroidProjects/E-comExpress/res/layout/offers_layout.xml<br>
Two files created for the implementation of offers feature. file offers_layout.xml created for the user interface and offers.java created for implementing logic for offers features.<br>
This will be used for implementing the feature of offers<br>
<br>--------------------------------------------------------------<br>

## Architecture
### Explain what a RESTful architecture is?
ReST(Representational State Transfer) is a software architectural style that defines a set of constraints to be used for creating web services. Web Services that conforms the ReST architectural style are called as ReSTful web services, provides the interporability  between computer systems on the Internet. RESTful web services allow the requesting systems to access and manipulate textual representations of web resources by using a uniform and predefined set of stateless operations. <br>
In ReSTful webservices , requests are made to the resource's URI, which sends the response as JSON , XML format. While the response conforms that some alteration has made to the stored resource and response can provide hypertext links to other resources or collection of resources. When HTTP is used, as it most comman, the operations available are GET, PUT, DELETE, POST and other CRUD HTTP methods.<br>
### How would you scale a slow website?
Our website performance is directly depends on the components of the websites that its using like images, javascripts, CSS and so.
To scale a slow website , we can do following things:
Studies show that web page response time can be improved by 25 to 50 percent by following these rules:

    Minimize HTTP requests.
    Use a content delivery network.
    Add an Expires or a Cache-Control header.
    Gzip components.
    Put stylesheets at the top.
    Put scripts at the bottom.
    Avoid CSS expressions.
    Make JavaScript and CSS external.
    Reduce DNS lookups.
    Minify JavaScript and CSS.
    Avoid redirects.
    Remove duplicate scripts.
    Configure ETags.
    Make Ajax cacheable.
    Use GET for Ajax requests.
    Reduce the number of DOM elements.
    Eliminate 404s.
    Reduce cookie size.
    Use cookie-free domains for components.
    Avoid filters.
    Do not scale images in HTML.
    Make favicon.ico small and cacheable.
    
### Your application just got millions of users overnight, what do you do?
We can do following things in such scenarios:<br>
#### Plan to Future: <br>
#### Web/App Architecture:<br>
#### Ready to Support:<br>
#### Scale up:<br>
#### Monitoring:<br>
#### Storage Space addition:<br>

### What are the advantages and disadvantages of implementing a Microservices architecture?
#### Advantages of Microservices architecture:
<b>Scaling:</b> It is very easier to scale the microservices applications which is being used more. <br>
<b>Resilience:</b> In Microservices architecture , if one service goes down, it will effect the other services in the system.The other part of the system will keep working as usual.<br>
<b>Technology Mix:</b> With microservices, its not necessary to keep stick with the single techonology. You can Mix any other technology with microservices.<br>
<b>Easy Deployments:</b> In microservices architecture , if done correctlly, helps in making the deployment process smooth.<br>
<b>Easy Modifications:</b> Whenever requirement changes and need some modifications in the application, With microservices architecture , it is very easy. as we just need to change/modify the particular service not the whole application. <br>
<b>Rollbacks:</b> If anything goes wrong, rollbacks in microservices architecture is very easily and quickly. <br>

#### Disadvantages:
<b>Dependencies Problem:</b><br>
As we can use more than one language in microservices architecture, We need to manage, handle, test all the dependencies with respective language.<br>
<b>Non Uniform Service Abstraction:</b><br>
In webservices, it is possible to have multiple langauages, hence the application does not have a uniform service abstraction.<br>
<b>Multiple DBs and Transaction Management:</b><br>
As there are more than one services running at a time, We need to handle and manage all the concurrent services DBs and Tranasactions.<br>
<b>Testing:</b><br>
The testing of microservice is very hassel task as it comes with various aspects of Testing , while the room for end-to-end Testing is challenging task.<br>
<b>Necessary Monitoring:</b><br>
<b>Decreased Performance:</b><br>
<b>Increased Memory Consumption:</b><br>
<b>Deployment Complexity:</b><br>
<b>Teams Communication Overhead:</b><br>
<b>Formal Documentation Overhead:</b><br>
<b>Devops Complexity:</b><br>
<b>Increased network Communication:</b><br>
<b>Marshalling and Un-Marshalling :</b><br>
<b>Network Security:</b><br>
<b>Production Monitoring:</b><br>

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
## Security
### What is the importance of SSL?
SSL is backbone of secure Internet. It Stands for Secure Socket Layer. Nowdays, it is most important and mandatory for most of the websites such as e-commerce sites. SSL provides various advantages to your site, they are as follows:
#### 1. Encrypt Sensitive Information
As we know that, whenever we submit our sensitive information such as credit card information, this information is travelled across the internet and at the end provided to the intended user like an e-commerce company. While this information is passes through such large numbers of computers, it is possible that some middle computers may revealed this information to unintended persons. Hackers can get such information and can do any kind of harmful activity. Hence such information has to be secured and only made available to the intended user. We can achieve this by using SSL. SSL provides strong encryption to such information and can only be available to the user who has valid decrytion keys.  SSL encrypt such information and then send it to the server, while if Man-In-Middle Attack happens and hacker eventually get this information , it will totally unreadable because of its encrypted form. 
#### 2. Provides Authentication
While using SSL, it will provide the assurity to the user that they are connected to the right website.
#### 3. Guard against Phishing
SSL protect against the phishing attacks because it very difficult for malicious user to get the SSL certificate as it goes through the various security checks to get the SSL certificates.
#### 4. Customer Confidence
If you are using SSL for your site, almost all browsers will show the green bar at address bar or some green lock icon to show that the site which users are visiting is secured and customers or your site visitors can sure that the information they are submitting is secure. <br>

## Cloud
### Which cloud providers are you familiar with?
- AWS
## What are the benefits of using a cloud provider?
To check out the benefits of cloud, we need to consider the limitations of our own set of servers.<br>
<b>1. Initial Setup / Requirement </b><br>
<b>2. Configuration </b><br>
<b>3. Space Requirement </b><br>
<b>4. Maintainance </b><br>
<b>5. Scaling issues </b><br>
<b>6. Decommisioned Servers </b><br>
<b>7. Cost </b><br>
<b>1. Initial Setup / Requirement </b><br>
Whenever we are going to setup new servers on our own , we need to consider our requirements first. Like the Disk Size of the server, RAM, NICs and much more. And this is the manual activity which takes more time to takes place. While the business growth doesen't allows that much time lapse to provision the server which may be result into the business loss.<br>
<b>2. Configuration </b><br>
Once our server setup is done, after that we need to configure our server with some specific configuration that we required to launch our application etc. Again this is also the time consuming process and think that we need to configure some 100s of server with same configuration. That case , provisioning this much servers takes days or weeks.<br>
<b>3. Space Requirement </b><br>
To provision our own server, we need some physical space for that. which again came an issue when we don't have enough space on our areas.(Physical Server Locations).<br> 
<b>4. Maintainance </b><br>
Wnenever we have our own servers, we need to do regular check and maintainance for those servers.Where we need some human resources to keep track of such things. Which may again come in the result of increased cost.<br>
<b>5. Scaling issues </b><br>
At some point of time , we need to provision more servers with same application running on it. Like consider that we have a web application and on weekends we gets lot of traffic on our site. That case we need to provision more servers. But to provision servers with such a limited time span is a very challenging task and if may result into failures then produces major issues.<br>
<b>6. Decommisioned Servers </b><br>
Once some project/ Software development done where we are using our servers and now they don't required those servers. That decommisioned servers are again burden to the organization because even they are not in use but we need to keep there maintainance.
And we need to wait for some situation where we can again use those servers.<br>
<b>1. Cost </b><br>
Lots of cost is involve in maintaining such servers starting from physical space requirement to the maintainance, And also need some human resources.<br>
Cloud providers will do these all things for us, so that we can focus on our business goals. Cloud providers offers on-the-fly VM creations, provides built in configurations or we can create our required configuration very easily and once this done, will can focus once our application rather than it's Provisions on servers. Not only these , Cloud Providers also offers some built in tools for managing such servers on the go.<br>


## Have you managed production systems in the past?
- No
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

## General
### Which Software Stack do you use and why?
I have worked on some of the software stacks, they are LAMP(Linux, Apache, MySQL, PHP) , WINS(Windows Server, Internet Explorer, .Net, SQL Server). along with these two Linux and Windows Platform stacks, I also worked on ELK(ElasticSearch, LogStash, Kibana) Stack, Which is mostly used for log management and analysis.<br>
As on <b>Linux</b> , <b>LAMP</b> provides the all in one functionality for developing the website , web application and it is mostly used over the world. The big reason behind it's usage is , it's totally open source. (Linux is an open source Operating System Distribution, Apache is free and open source web Server, MySQL is one of the most famous and free Relational Database Engine, PHP is general purpose Server Side Scripting language).<br>
On <b>Windows</b> platform, <b>WINS</b> provide full features and functionality for development on Windows Platform. While WINS Software stack is Proprietary Softwares. But This provides full support on windows Platform. By using WINS Stack ,Moslty standalone applications are being developed which are natively works on Windows.<br>
Coming to <b>ELK</b> Stack,Which is mostly used for <b>log analysis and management</b>, Is also an open source software stack. Where Elasticsearch is acts as a powerfull search engine which is responsible for searching the required data from the large collection of Data. Logstash will acts as a collector and storage engine, and Kibana provides beautifull and user friendly interface for Data Visualization.<br>
While there is lots of other tools can be used with ELK Stack like filebeat, Metricbeat and so on.

### Describe your worst Fear?
I'm Fearless person. I'm not afraid of any kind of fear like failures. Because I believe in my hard work, and I believe that hard work will soon pay off . Someone says,If you fail 10000 times don't consider it as failures, consider it has , you learn 10000 ways that it won't work.<br>

### What new technology would you like to learn?
I would like to learn Hadoop with DevOps Prospective. As we know that Hadoop deals with <b>"Big Data"</b> Techniques and can process petabytes of data in seconds. While the increasing database in Hadoop cluster, It needs more and more nodes to store this data and this distributed dataset is sometimes challange to the Server administrator. Combining DevOps for Hadoop is somewhat challenging thing but these both are latest trends in the market with increasing popularity day-by-day and definitely future of tomorrow's IT world.<br>
This article on web inspired me lot towards learning Hadoop with DevOps.<br>
https://community.hortonworks.com/articles/108610/hadoop-devops-better-together.html

### Do you contribute to any open source projects?
NO.
