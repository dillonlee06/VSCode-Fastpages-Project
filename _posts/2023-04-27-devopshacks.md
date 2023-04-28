---
toc: true
layout: post
categories: [AP Notes, CSP Assignments]
title: Devops Hacks
---
# Introduction:
## Introductory Question
> In 2-3 sentences, explain the purpose of DuckDNS as a DNS alternative to what is already in place (Freenom). Do you think we should use one or the other? Why or why not?
- Answer: Users can link a domain name to an IP address using the free DNS service offered by DuckDNS. It can be used in place of Freenom, which also provides free domain names. When deciding, it is important to consider the different pros and cons regarding user friendliness, accessibility to domain extensions, customer service, etc

> Sample Answer:
- DuckDNS provides a free dynamic DNS service that allows users to assign a domain name to a dynamic IP address. It can be used as an alternative to Freenom, which also offers free domain names. The choice between the two depends on individual needs and preferences, such as ease of use, availability of domain extensions, and customer support.

# FRQ
> Complete the answers in your own words
- Question 1: How does AWS Work?
- AWS works by providing a cloud computing platform that allows users to access a wide range of infrastructure and application services on a pay-as-you-go basis. AWS operates on a global scale, providing high availability and scalability for its customers.
- Question 2: How is AWS useful for projects?
- AWS is useful for projects because it provides a wide range of infrastructure and application services that can be used to build, deploy, and scale applications quickly and easily. AWS also allows users to only pay for the services they use, making it cost-effective and scalable for projects of all sizes.
- Question 3: How does Duck DNS Work?
- Duck DNS works by providing a way to assign a domain name to a dynamic IP address. Users can create an account with Duck DNS, configure their router or device to update their IP address with Duck DNS, and then access their device using a domain name that points to their current IP address.
- Question 4: How is Duck DNS useful for projects?
- Duck DNS is useful for projects because it allows users to access their device using a domain name that points to their current IP address, even if the IP address changes frequently. This makes it easier to access the device remotely and also enables services to be hosted on devices with dynamic IP addresses.

# Section Hacks

## HACKS FOR KASM
> In 3-4 sentences, please explain the significance of virtual desktops and KASM. How can virtual desktops such as these be utilized in our AP CSP environment? (0.45)
- Users can access their PCs from any location with an internet connection by using virtual desktops like KASM. This is important because it enables users to access their documents and software without physically being in front of their computer, which is advantageous for both convenience and security. In an AP CSP setting, virtual desktops can be used to provide students with access to software and programming environments that they might not have on their personal devices and to establish a uniform and secure computing environment for all students.

## Alternatives to Certbot Hacks
> Research and compare the security features of OpenSSL and LibreSSL, and write about the recent vulnerabilities within it. Write about your research in a fastpages blog post. It can be the same post that has your screenshot for the Certbot Hacks.
- OpenSSL and LibreSSL are open-source implementations of the SSL and TLS protocols used to encrypt data in transit over a network.
- LibreSSL is a fork of OpenSSL that was created after the discovery of several critical vulnerabilities in OpenSSL, which led to a major overhaul of the codebase to improve security.
- Recent vulnerabilities in OpenSSL have included Heartbleed, which allowed attackers to steal sensitive information from memory, and CVE-2021-3712, which allowed attackers to cause a denial of service or execute arbitrary code.

## EC2 AWS Hacks
> FRQ Question Hacks (Answer with more than 2-3 full complete sentneces):
- Are there any outdated Nginx/Docker functionalities to address?
- To make sure that the software used in a project is current and secure, it is always advised to check for the most recent versions of Nginx and Docker. By updating to the most recent version, any out-of-date features should be fixed.
- Is there anything unclear that we need to communicate further to the students for deployment?
- I am an AI language model, thus I am unsure of the details of the deployment you are referring to. To enable me to respond appropriately, please provide me some details about the project or task.

> Diagram
- To Truly understand Nginx and why we are using it, it is important to compare it to other web servers? Compare NGINX with lighttpd in a Venn Diagram, and place the image below:

![]({{site.baseurl}}/images/NGINX vs lighttpd.png "Venn diagram")


## Duck DNS HACKS
> HACK 1 - Create a diagram (canva)
- ![]({{site.baseurl}}/images/7.png "14")

> What are the pros and cons of using Duck DNS
- ans

HACK 2 - Write a reflection

- Why do we use DNS?
- How does Duck DNS work?
- What makes Duck DNS unique?
- How is Duck DNS useful for our projects?
- What are the steps to set up Duck DNS?


## Guide to SQLite vs AWS alternate databases Quiz
> What is the main difference between relational and non-relational databases?

A. Relational databases are only used for structured data, while non-relational databases are only used for unstructured data.

B. Relational databases can easily handle high data volumes, while non-relational databases cannot.

C. Relational databases are based on tables and use SQL, while non-relational databases are based on collections and use JSON-like documents.

D. Relational databases are more expensive than non-relational databases.

> Which AWS database service is best suited for applications that require low-latency speed?

A. Amazon ElastiCache

B. Amazon Neptune

C. Amazon DocumentDB

D. Amazon RDS

> What is the purpose of the code example provided in the lesson?

A. To demonstrate how to create a table in Amazon Aurora.

B. To show how to query data from a DynamoDB table.

C. To provide an example of how to connect to a database instance in RDS using Python.

D. To showcase how to insert data into a MySQL table.
