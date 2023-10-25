# What is a Virtual Private Cloud (VPC)?

A Virtual Private Cloud is an isolated private cloud located within a public cloud which separates a user's resources from others within the same network. A customer can use a VPC to do many things including (but not limited to): hosting websites, running code and storing data. 

![image](https://github.com/g-sreshtha/networking-notes/assets/146075375/06c50c94-ce82-4871-a3b8-505f6465f096)
***source: https://geekflare.com/virtual-private-cloud/***

## Definitions
- **Public Cloud**: This is a platform managed by a third-party company that uses ***the standard cloud computing model*** to make services available to remote users around the world and is usually accessed over the Internet. This allows flexibility and scalability as well as creating a broad network access. Some examples of popular public cloud services are:
        <ul>
                <li>AWS</li>
                <li>Microsoft Azure</li>
                <li>Google Cloud</li>
        </ul>
- **Private Cloud**: This is a cloud computing environment dedicated to a single customer provided by a private organisation. This makes all hardware and software recources within the environment exclusively accessible to a single user which allows the benefit of control of on-premises IT infrastucture as well as increase security. One may choose a private cloud to deal with:
        <ul>
                <li>Confidential documents</li>
                <li>Intellectual property</li>
                <li>Medical Records</li>
                <li>Financial data</li>
                <li>etc.</li>
        </ul>
Despite such benefits for both public and private clouds, private clouds can come with a higher cost whereas public clouds can compromise on meeting regulatory compliance requirements.
## The Standard Cloud Model
![image](https://github.com/g-sreshtha/networking-notes/assets/146075375/a601ccaa-4a6e-4cad-b377-02c51644f333)
***source: https://www.slideteam.net/standard-cloud-service-models-cloud-computing-service-models.html****
## How does a VPC work?
Through the allocation of private IP subnet and a virtual communication construct such as a VLAN or a set of encrypted communication channels per user, the isolation between one VPC user and their resources and all other users within the same public cloud can be achieved.
- **Subnets**: This is a network within another network which makes transferring data more efficient by causing network traffic travel shorter distances without passing through unnecessary routers to reach its destination. It is made up of a range of IP addresses within a network to be able to divide a part of it for private use. In a VPC, private IP addresses are used that are not accessible via the public internet so resources can be kept private. 
- **VLAN (Virtual Local Area Network)**: This is a custom network created from one or more local networks which enables devices in multiple networks to be combined into one logical network without the use of the internet. It works like a subnet to partition a part of the network however it functions in a different layer of the ***OSI Model***. The subnet partitioning occurs in the second layer, whereas the VLAN partitioning often happens in layer 3.
- **VPN (Virtual Private Network)**: This uses encryption to create a private network over the top of the public network. Depending on the VPC, a different type of encryption can be used to protect the data including:
    - AES encryption
    - Public Key Encryption
    - Symmetric Encryption
    - Transport Layer Security
## OSI Model
![image](https://github.com/g-sreshtha/networking-notes/assets/146075375/8b25b433-167b-4568-81aa-bead8ed629aa)
***source: https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/***

## Advantages and Disadvantages

## Why use a VPC?
