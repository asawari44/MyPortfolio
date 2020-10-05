---
title: "Amazon web services : Containers and Fargate"
date: 2020-09-28T12:14:34+06:00
image: "images/blog/post-1.jpg"
description: "In the cloud arena, Container technology is growing tremendously after the release of Docker back in 2013. The objective of the technology is to deploy applications in the form of microservices on a larger scale, more efficiently, without unnecessary delays and with reduced cost.  In recent years, multiple cloud providers such as Amazon, Azure, Google Cloud Platform, etc have introduced container orchestration technologies. AWS Fargate is one of them and it leverages underlying container services provided by AWS."
draft: false
---
## Introduction 

In the cloud arena, Container technology is growing tremendously after the release of Docker back in 2013. The objective of the technology is to deploy applications in the form of microservices on a larger scale, more efficiently, without unnecessary delays and with reduced cost.  In recent years, multiple cloud providers such as Amazon, Azure, Google Cloud Platform, etc have introduced container orchestration technologies. AWS Fargate is one of them and it leverages underlying container services provided by AWS.  
To comprehend the discussed technology, it requires some basic understanding of container orchestration and microservices on public cloud platforms such as AWS or Azure. After reading the document, the reader is expected to understand AWS Fargate technology and it’s basic functioning. Also, its evolution, competitors, future plans should be apparent from the document. 
In the 3rd section, the impacts are not the direct effect of the discussed technology but the company providing the discussed service is assumed to have larger and more concrete impacts. Hence, the impacts are generic. It’s an assumption that any service or technology built or provided by Amazon would add on to the company’s existing political, social, legal and environmental impacts.
As an author of the report, I would like to thank EIT digital masters program and Professor Kent Thorén for creating valuable content(online modules, regular teaching sessions) that helped me analyze the technology from different perspectives. 
 
## Technology 

AWS Fargate is a technology used by Amazon web-services in two container-based services namely AWS elastic container service and AWS elastic Kubernetes service. Fargate is used to manage container orchestration in a serverless fashion. In container orchestration technologies, it is typical to create virtualized infrastructure before creating containers on top. In Fargate, there is no need for managing the underlying infrastructure. Users only need to pay for the amount of compute used in order to spawn and run microservices on containers. This saves users from the trouble of choosing instance type and storage for creating infrastructure from scratch on AWS. It is also an economically viable option as users pay exactly for what they use. Fargate provides a strictly isolated environment for containers to run and thus claims that the microservices remain highly secure, even though the user does not have complete control over the underlying virtual machines. It manages application deployment in terms of tasks. For each task, it allocates a safe and isolated environment and launches the task definition in the form of a container. With this service, users can mainly focus on developing applications and less time goes into handling the infrastructure. Depending on the type of application, a specific subscription model can be chosen. For example, on-demand prices for time-critical applications are high, whereas Fargate offers a 70% discount[1] on the prices for fault-tolerant applications. 
 
## A wider perspective of the selected technology 

AWS Fargate is a relatively new technology that leverages currently present container orchestration solutions. It brings about many changes in the way microservices are utilized and has impactful effects in the economical sense. Major impacts in terms of different perspectives can be stated as below-  
Politics: There is no direct impact of the newly introduced technology/service but speaking about Amazon as a company, there has been recent news about the American president, Donald Trump trying to influence the Joint Enterprise Defense Infrastructure (JEDI) contract between Azure and Amazon, according to the sources mentioned in the article[2].
Economics: This is the biggest area where the impacts of the newly created technology can be seen. Fargate allows users to pay for the containers and not for the infrastructure used to launch these containers. So, in the traditional scenario, a user would pay for the infrastructure even though all its resources are not fully utilized by the containers launched on top of it. Due to Fargate, businesses can save a lot of money over longer periods of time.   
Social: AWS services are quite mature and advanced as compared to many other public cloud providers. AWS has changed users and developers' perspective of leveraging cloud technologies. The services provided by the platform makes things faster, agile and easier to change for businesses. 
Technology: Although AWS Fargate uses container orchestration technology as its base, it’s an innovative addition to the existing stack of technologies, as it leverages container services in a new way.
Legal: AWS claims that all the services provided by it are GDPR compliant[3] and take user-data protection policies very seriously. 
Environment: Firstly, AWS plans to have all the available global infrastructure to be powered by renewable energy sources[4]. Secondly, The Fargate technology is based on containers which have a lower carbon footprint[5] as compared to virtual machines. Hence, dockerizing /containerizing applications is always a more environmentally friendly option as compared to deploying applications directly on the virtual machines.  

## Technology Delta
Kubernetes is a traditional way of container orchestration and Fargate utilizes the internal working concepts of kubernetes and leverages container technology. Kubernetes cannot be directly compared with Fargate, but Fargate can be considered a huge improvement over how container orchestration works. It is cost-efficient, serverless and easy-to-use as compared to Kubernetes. 
Azure container instances (ACI), a service equivalent to Fargate, is provided by Azure for container orchestration without having to deploy or manage servers or underlying infrastructure. There are almost no differences in the functionalities provided by both the services. Both have the same purpose but there are some nuances in terms of the internal working. ACI supports windows based containers whereas Fargate does not have explicit support for anything apart from Linux containers. On the other hand, Fargate provides a more mature and pretty-looking UI for managing container count and overviewing your infrastructure whereas ACI does not have a proper UI but containers can be managed from the CLI.  Secondly, performance-wise there isn’t a significant difference but from the experiment conducted in the article[6] Fargate seems to be more consistent in terms of response delays but the results could be highly dependent on the selected region for deployment. The pricing models for both ACI and Fargate are similar but considering the same application and the number of computational resources, Fargate is slightly more economical than ACI. 

## Entry Barriers

Nowadays, almost every large company is moving to cloud and microservices from traditional monolithic applications, where on-premise dedicated servers are maintained and tremendous amounts of manual work is needed. But if the application is already designed and deployed in a monolithic manner, there is a definite need of a complete revamp. Companies need engineers who are familiar with docker technologies and microservices to redesign and deploy their applications to suit the cloud deployment standards. Containers require docker images to boot, these images have inbuilt code and all the required packages to run the code.  Investment into this venture could involve research, a team of DevOps engineers, cloud consultants, etc, depending on the characteristics of the application.  Although if the company is already far too involved in microservices and cloud , there isn’t much of a barrier for moving to Fargate technology as it only changes a small process in the deployment phase of the application. 
Some of the competitors for AWS fargate can also make it difficult for the technology to be picked over others. For example, Azure kubernetes cluster, ironWorks also offer the similar functionality with lower container startup time hence companies which build windows based products would most likely prefer azure equivalent service over amazon Fargate as it would be easier for them to integrate it with other Azure services. 

## Future scenario 

Currently, Amazon has two main container orchestration services namely, Elastic Kubernetes Service (EKS) and Elastic Container Service (ECS). Fargate makes the management of these services easier. Yet it is only a start. The user still has to manage the capacity in the sense the number of containers needed to be launched. Auto-scaling rules are also defined manually and they are not always efficient as they have a statically defined threshold.  Eventually , AWS might decide to make EKS and ECS completely invisible to the user and expose only the managed Fargate service[6]. EKS still demands a user to form a cluster beforehand but with the managed Fargate service, there would be no need to even specify the number of cluster nodes in kubernetes. With this advancement, AWS would truly provide Container-as-a-platform service where managing serverless infrastructure, autoscaling, or even determining how many instances to launch how many containers to manage the workload would be entirely handled by AWS with the least human intervention. Thus, even though fargate removed the infrastructure handling problem, they still haven’t removed the capacity management scenario. If they manage to do that as well, it would make businesses even more economic and fast. 

## New possible business roles 

With the development in the existing AWS Fargate technology, cloud consultants and DevOps engineers have rising demands especially in the initial phase of the project. Their job is to advise businesses as to which service to pick based on the structure and the behaviour of the application. It is important to design the solution of what the architecture might look like is an extremely vital process in order to make cost-efficient business decisions in the longer run. With more applications moving to cloud, security is becoming a widely discussed topic. Cloud providers claim to provide a secure environment despite which data breaches are not uncommon. Most data breaches occur due to human errors, as configuring services on cloud requires human intervention. This creates a need to have DevSecOps and DevNetOps teams in companies. These teams are solely dedicated to handling security and network protection on cloud applications. To understand and implement AWS Fargate, it is important to have someone on the team with cloud and networking specialities along with AWS ecosystem understanding.  


## Early adopters for this technology 

After Fargate’s release, large companies like Accenture, Ancestry, Vanguard, Foursquare, Apple, 3M, NVIDIA, Silicon Valley Bank have moved their important and majority applications on AWS Fargate. Based on the testimonials[7] recorded by AWS Fargate customers, companies are moving to Fargate because they want to scale the environment quickly and it's a cost-effective and backward compatible solution. National Australian bank expects to have 75% cost reduction over a year after moving the banking application to Fargate. Apart from being cost-efficient, companies mention that Fargate enables easy DevSecOps, handles run-time memory and eliminates human intervention in mundane tasks. Anything that can be run inside a container without the need to manage the infrastructure can be easily moved to Fargate. BCI Chile, Mach claims that because of the managed services provided by AWS, the application did not suffer at all during the extreme peak times they observed after promoting the application. Serverless concept saves money, time and operational costs and most DevOps consultants are moving towards Fargate for these reasons. 
## Strategy for crossing the chasm
 
Even though AWS is a growing industry, they are very well-aware of the fact that consumer behaviour can change and chasms need to be taken seriously as they can help deal with the bandwagon effect which states that more number of people join the growing trend or fad if it starts growing, without considering the underlying evidence or logic. According to the published article by AWS[8], AWS has different ways of avoiding chasm and handling stagnant environments. They believe that there are different employee groups in every organization when it comes to the cloud and IT industry namely, innovators, early adopters , early majority, late majority and laggards. AWS suggests that each  group needs to be handled carefully to avoid chasm. For example, innovators should be pushed to get more interesting ideas in place. Early adopters should be allowed to run experiments on non-critical applications. Early majority should be pushed more to work on an intense project which should be publicized as much as possible to get the peer's attention. Late majority should be given opportunities for certification and low-risk participation programs to show long term support. laggards have their fears about the change so the best way to deal with them is to listen to their feedback without trying to sell them big ideas.

## References, web links
[1]https://aws.amazon.com/fargate/

[2]https://www.geekwire.com/2019/amazon-web-services-ceo-cites-significant-political-interference-trump-jedi-contract/

[3]https://aws.amazon.com/compliance/gdpr-center/

[4]https://sustainability.aboutamazon.com/environment/the-cloud?energyType=true

[5]Anusooya, G., Vijayakumar, V. Reduced carbon emission and optimized power consumption technique using container over virtual machine. Wireless Netw (2019)

[6]https://thenewstack.io/comparison-aws-fargate-vs-google-cloud-run-vs-azure-container-instances/

[7]https://aws.amazon.com/fargate/customers/

[8]https://aws.amazon.com/blogs/enterprise-strategy/drive-change-but-avoid-the-chasms/
