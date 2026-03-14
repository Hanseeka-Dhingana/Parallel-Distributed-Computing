# Computing and Computing Trends
## What is Computing?
At its core, computing is any activity that uses computers to manage, process, and communicate information. The evolution of computing has moved from standalone machines to highly interconnected systems .

## Trends in Computng?
### 1. What is Distributed Computing?
Distributed computing is a system where a group of autonomous computers works together to appear as a single computer to the end user.

* **How it works:** Each computer (or processor) has its own local memory. They don't share memory directly; instead, they communicate with each other by passing messages through communication lines like high-speed buses or networks.

* **Key Components:** A typical distributed system consists of **Workstations** for end-users, **Server Systems** to provide resources, and **Personal Assistance Devices** (like handheld devices) connecting via wireless links.  
![](assets\DistributedComputing.png)

#### Why do we need it? (Key Properties & Benefits)
* **Fault Tolerance & Robustness:** There is no Single Point Of Failure (SPOF). If one node fails, the rest of the system can keep working (though performance might dip), and other nodes can take over the failed node's tasks.

* **Resource & Load Sharing:** Users can share computing power and storage across the system, and tasks are dispatched to different nodes to balance the system's load .

* **Scalability or Easy to Expand:** It is very easy to expand; you can add new nodes with minimal to no downtime.

* **High Performance:** It is excellent for "Compute-intensive" tasks (like Monte Carlo simulations) and "Data-intensive" tasks (like processing data for Facebook or the Large Hadron Collider) .

* **Each Node Plays a Partial Role** In a distributed system, there is no single "all-knowing" computer. Each computer only has a limited, incomplete view of the entire system. Because the system is so large, a single node might only know its own specific part of the input data and nothing else.

#### Real-World Applications & Examples (Use-case)
* **The Internet:** The ultimate distributed system, where millions of autonomous servers and clients share information globally.

* **ATM Machines:** ATMs are distributed nodes. *Real-life context:* When you withdraw cash in one city, that ATM (a local node) communicates via message passing to a central bank server to verify your balance, deduct the funds, and authorize the cash dispense, all while appearing as one seamless banking experience to you.

* **Intranets/Workgroups:** A company's internal network where employees share files and printers across different departments.

#### How Distributed Software Applications Work
* A distributed application is a software program that consists of a set of processes distributed across a network of machines. These machines work together as an ensemble to solve a common problem.

* **1. The Old Way (Client-Server):** In the past, most distributed apps were built on a "client-server" model. In this model, the resource management is centralized at the server.

* *Real-Life Example:* A standard multiplayer video game. You (the client) move your character, but the main game server does all the heavy lifting and tells everyone else where you moved. If the server crashes, the game ends for everyone.
![](assets\ClientServer.png)
* **2. The "Truly" Distributed Way (Peer-to-Peer):** The slide notes that "Peer to Peer" (P2P) computing represents a movement toward more "truly" distributed applications. In a P2P network, there is no central boss (server); all computers (peers) share the load and talk directly to each other.
* *Real-Life Example:* **BitTorrent** or **Bitcoin/Blockchain**. If you download a file using a torrent, you aren't downloading it from one central server. You are downloading tiny pieces of that file from hundreds of other users' computers (peers) all over the world at the same time. This makes it "truly" distributed!
![](assets\Peer2Peer.png)

### Centralized Computing VS Distributed Computing
#### Centralized Computing
* **The Concept:** This refers to early computing where tasks are performed on a single processor, which is also called uni-processor computing. In centralized systems (like classic "client-server" models), all resource management is centralized at the server.

* **Real-Life Example:** Think of an old-school retail store checkout system from the 1990s. There is one main computer (the server) in the back office, and all the cash registers out front are just "dumb terminals." The registers have no processing power of their own; they just send input to the back-office computer. If that one back-office computer crashes, every single cash register in the store stops working because there is a Single Point of Failure.

#### Distributed Computing
* **The Concept:** This is a group of computers distributed across a network. Instead of one machine doing all the work, these independent machines work together as an ensemble to solve a common problem. To the end-user, it appears as if they are interacting with just a single computer.

* **Real-Life Example:** Think of **Google Search**. When you hit "search," you aren't asking one massive centralized computer to find your answer. Your request is split up and handled by a distributed network of thousands of servers working together as a team. Because it's distributed, if ten Google servers randomly lose power, your search still goes through instantly because other nodes pick up the slack.  
![](assets\CVD.png)    


###  What is Cluster Computing?
A cluster is a type of parallel or distributed computer system. It is a collection of inter-connected stand-alone computers that work together so closely they appear as a single, integrated computing resource.
* **The "Tightly-Knit" Difference:** Unlike standard distributed networks (which might connect computers across the globe via the internet), a cluster's computers are usually in the same room. They are connected by a network that is much faster and closer than a typical LAN, using "low latency" (super fast, zero-delay) communication protocols.

* **Key Components:** It involves multiple standalone computers, operating systems, high-performance interconnects (the cables), middleware (the software that links them), parallel programming environments, and applications.

*Real-Life Example:* Imagine one horse trying to pull a massive wagon. It can't budge it. But if you tightly harness 10 strong horses together to pull at the exact same time, they act as one giant, powerful engine. That harness is the "high-performance interconnect," and the horses are the "cluster."

#### How it works
A cluster typically works using a master-worker relationship:
1. **The Root Node (The Master):** The input data is sent to the main computer, called the root node.

2. **The Slave Nodes (The Workers):** The root node chops the big task into smaller pieces and delegates them to the connected computers, known as slave nodes (node 1, node 2, node n).

3. **The Result:** The slave nodes do the heavy lifting simultaneously and send their answers back to the root node, which pieces everything together to give you the final result.

#### Types of Clusters
* **High Availability (Failover) Clusters:** These are designed so the system never goes down.

* *Example:* A hospital's electronic patient record system. If the primary server crashes, the backup server in the cluster instantly takes over (fails over) so doctors never lose access to critical medical data.

* **Load Balancing Clusters:** These distribute incoming traffic evenly across all the computers in the cluster.

* *Example:* The Sukkur IBA student portal on the day exam results are released. Thousands of students log in at once. The cluster balances the requests across 10 different servers so no single machine crashes from the pressure.

* **Parallel/Distributed Processing Clusters:** These are used to solve massive computational problems by splitting the math across all nodes.

* *Example:* Rendering a 3D animated movie. The cluster splits the movie's frames across hundreds of computers to process them in parallel, finishing a job in days that would take a single PC years.

#### Benefits of a Cluster
Because of how they are built, clusters offer some massive advantages:

* **System Availability & Reliability:** The system is highly available because there is a redundancy of hardware, operating systems, and applications. You can run multiple copies of the OS and apps, so if one fails, the others keep running.

* **Hardware Fault Tolerance:** They use redundancy for most system components (like disk-RAID), meaning if a hard drive physically breaks, no data is lost.

* **Scalability:** If your company grows, you don't need to throw away your system; you just add more servers to the cluster as the need arises.

* **High Performance:** Combining all these machines simply gives you massive, supercomputer-level computing power.


### What is Grid Computing?
Grid computing links together computing resources (like PCs, servers, and storage) to create a single, massive "virtual" computer.
* **How it works:** Users access processing power, network bandwidth, and storage capacity without needing to know where the hardware is actually located or what operating systems are running.
* **The Magic Trick (Scavenging):** One of the coolest parts of a grid is that it harnesses the *unused processing cycles* of regular computers in a network.
* *Real-Life Example:* Imagine an office with 1,000 desktop computers. At 5:00 PM, everyone goes home, but the computers stay on. A Grid Computing system will "borrow" the processing power of those 1,000 sleeping computers overnight to solve a massive scientific math problem!

#### 1. The Need for Grid Computing
* **Complex Science & Research:** Modern science relies heavily on deep data analysis, massive computations, and collaboration.
* **Cost Effectiveness:** Running a computer simulation on a grid is much cheaper than building real-world physical experiments.
* **Speed & Accuracy:** Problems in engineering and science are getting incredibly complex. We need highly accurate solutions in the shortest possible time.
* **Efficiency:** As mentioned above, it exploits under-utilized resources (like sleeping office PCs) so computing power doesn't go to waste.

#### Real-World Applications
* **Weather Forecasting:** Crunching atmospheric data from thousands of sensors worldwide to predict global weather patterns.
* **Detection and Modeling of Natural Disasters:** Simulating how a tsunami will travel across the ocean so early warnings can be issued.
* **Physics Applications:** *Real-Life Example:* The Large Hadron Collider (LHC) generates millions of gigabytes of data. They use a massive global grid to distribute that data to physicists all over the world for analysis.

#### Types of Grid Computing
* **Computational Grid:** Focused on pure processing power. Used for High-Throughput Computing (HTC) and High-Performance Computing (HPC) . *(Example: Borrowing CPU power to simulate how proteins fold to cure diseases).*
* **Data Grid:** Focused on managing, sharing, and storing massive volumes of data across different locations . *(Example: A network allowing universities across the country to instantly access a giant database of genetic research).*
* **Collaboration Grid:** Designed to handle advanced collaboration over the internet . *(Example: Engineers in Pakistan and Germany simultaneously working on and interacting with a live 3D model of an airplane engine).*
* **Network Grid:** Provides fault-tolerant and high-performance communication services .
* **Utility Grid:** The ultimate form of the grid. It doesn't just share data or processing power; it shares *everything*—software, storage, and any other resource.

### What is Utility Computing?
It is a "service provisioning model". This means instead of a company buying their own expensive physical servers, a service provider gives them computing resources and manages the infrastructure for them as needed.

* **The Name:** It is called "utility" because it works exactly like traditional public utilities such as electrical power, water, gas, or telecommunications.
* **The Core Concept:** You don't buy the power plant; you just plug into the wall and pay for the exact amount of electricity you use. In computing, this is known as a "pay-per-use" or pay-for-use pricing business model.

### How the Payment Model Works
Just like your mobile phone or electricity bill, utility computing offers a range of charging models:
* **Pay as you go / Metered:** You are charged exactly for the gigabytes of storage or processing power you consume that month.
* **Subscription / Flat rate:** You pay a set fee every month for a specific tier of service.
* Providers will offer different pricing models based on the scale of the customer's needs, their commitment length, and how frequently they pay.

#### Why is it useful?
* **Solves Resource Utilization:** If a company buys 10 servers but only uses 2, that is a huge waste of money. Utility computing solves this because you outsource the IT function and only use (and pay for) exactly what you need at any given moment.
* **Data Center Virtualization & Web Services:** It relies on delivering these resources over the web dynamically.

#### Real-Life Example
Think about a small startup company launching a new mobile app.
* Instead of spending $50,000 to buy physical servers and put them in a closet, they use a utility computing service (like Amazon Web Services or Google Cloud).
* In month one, they only have 100 users, so their "utility bill" for server usage is only $10.
* In month two, their app goes viral and hits 1 million users! The service provider automatically turns the "tap" on to give them more computing power so the app doesn't crash. Their bill for month two goes up to $1,000, but they only paid for exactly what they consumed.  


---


## Core Definitions of Cloud Computing
* **Oxford Dictionary:** The practice of using remote servers hosted on the internet to store, manage, and process data instead of a local server.

* **NIST Definition:** A model for enabling ubiquitous, on-demand network access to a shared pool of configurable computing resources (networks, servers, storage, etc.) that can be rapidly provisioned with minimal effort.


## Cloud vs. On-Premise Computing
This highlight why businesses are shifting to the cloud by comparing it to traditional on-premise setups:

* **Cost & Scalability:** On-premise requires higher pay and offers less scalability, while cloud follows a "pay-for-what-you-use" model.

* **Maintenance:** Cloud removes the need for physical server space and dedicated hardware maintenance teams.

* **Security & Recovery:** Cloud typically offers better data security and more reliable disaster recovery compared to on-premise systems.

* **Flexibility:** Cloud allows teams to collaborate from widespread locations with rapid implementation times.


## Essential Characteristics 
1. **On-demand self-service:** Users can get resources without human intervention.

2. **Ubiquitous network access:** Resources are accessible from anywhere over the internet.

3. **Location-independent resource pooling:** Providers share resources across many customers.

4. **Rapid elasticity:** Resources can be scaled up or down quickly as needed.

5. **Measured service:** Users only pay for what they consume (Utility-based).

## Cloud Models
The categorizes the cloud into two main frameworks:
### 1. Deployment Models
* **Public Cloud:** Owned by a provider and made available to the general public (e.g., AWS, Azure).

* **Private Cloud:** Operated exclusively for a single organization.

* **Hybrid Cloud:** A combination of public and private functionalities.

### 2. Service Models

* **IaaS (Infrastructure as a Service):** Provides basic computing infrastructure like virtual machines (e.g., Amazon EC2, Google Compute Engine).


* **PaaS (Platform as a Service):** Provides a platform for developers to build, test, and manage applications (e.g., Google App Engine, Azure).


* **SaaS (Software as a Service):** Subscription-based software hosted by a vendor (e.g., Office 365, Google Apps).

## Advantages and Disadvantages

| **Advantages** | **Disadvantages / Concerns** |
| --- | --- |
| Lower computer and software costs |Requires constant, high-speed internet |
| Improved performance and boot speeds |Potential security and data loss risks |
| Unlimited storage capacity |Limited features in some web-based apps |
|Easier group collaboration |Lack of standard APIs between providers |  


## Typical Computing Patterns
The four typical computing patterns based on how much computer power (Compute) a business needs over time.
### 1. On and Off Workloads (Batch Jobs)
* **The Concept:** Your business only needs heavy computing power for a short, specific amount of time (like running batch jobs), followed by periods of complete inactivity.

* **The On-Premise Problem:** If you buy your own servers, you are paying for them 24/7. When they are "off," you are suffering from **wasted capacity**. Plus, buying and setting up these servers takes a long time, meaning your **time to market can be cumbersome**.

* **Real-Life Example:** An accounting firm that only needs massive computing power on the 30th of every month to process payroll.
* **The Cloud Fix:** You simply turn the cloud servers "on" for payroll day, pay for those 24 hours, and turn them "off" when you are done.

### 2. Rapid Growth
* **The Concept:** Your business is taking off and growing incredibly fast, meaning your need for computing power is constantly shooting upward.

* **The On-Premise Problem:** It becomes a **major challenge for the IT department to keep up with growth** because buying and installing physical servers takes months. If the servers can't handle the new users, the system crashes, leading to **potential customer service problems** and a **potential loss of business opportunity**.

* **Real-Life Example:** A brand new social media app that suddenly goes viral and gets a million new sign-ups in a week.
* **The Cloud Fix:** In the cloud, you can just click a button to add more servers instantly as your user base grows.

### 3. Unpredictable Bursting
* **The Concept:** Your daily traffic is usually flat, but out of nowhere, you get an **unexpected peak in demand**.

* **The On-Premise Problem:** You are trapped. If you didn't buy enough backup servers, your site crashes and you suffer a **loss of business opportunity**. If you panic and buy a ton of expensive backup servers *just in case*, you end up with **wasted capacity if demand wanes** (goes back to normal).

* **Real-Life Example:** A small clothing website that suddenly gets mentioned by a massive celebrity on a late-night talk show, causing thousands of people to visit the site at exactly midnight.
* **The Cloud Fix:** Cloud Auto-scaling. The cloud automatically detects the sudden traffic spike, spins up extra servers for the 3 hours you need them, and deletes them when the traffic leaves.

### 4. Predictable Bursting
* **The Concept:** You have **seasonal peaks and troughs** in your traffic. Unlike the previous pattern, you know exactly *when* the spikes are going to happen.

* **The On-Premise Problem:** This creates the **"Provisioning dilemma"**. Do you buy enough physical servers to handle the peak, resulting in **wasted capacity** for the other 11 months of the year? Or do you save money by buying fewer servers, resulting in a **loss of business** because your site crashes during your busiest season?

* **Real-Life Example:** A flower delivery website (massive spike on Valentine's Day and Mother's Day) or an e-commerce store during Black Friday.
* **The Cloud Fix:** You run a small number of cloud servers normally, and pre-schedule a massive expansion of servers specifically for the week of Black Friday, paying only for the extra power during that week.



## Technical Disadvantages of Cloud Computing
### **1. Limitations with Supercomputing (HPC)**
* **The Concept:** It is not entirely clear if you can efficiently run compute-intensive High-Performance Computing (HPC) applications that rely on specific frameworks like MPI or OpenMP in the cloud.


* **Simple Explanation:** Standard cloud servers are amazing at hosting websites or storing files. However, if a scientist needs to run a massive, highly complex mathematical simulation (like modeling a hurricane or rendering a 3D movie), standard cloud servers might struggle. They aren't always wired together in the ultra-fast, specialized way that supercomputers are.
* **Real-Life Example:** Imagine renting a standard delivery van to compete in a Formula 1 race. The van is highly useful for everyday tasks, but it isn't built for specialized, extreme-performance racing.

### **2. The "Vendor Lock-In" Problem (Different APIs)**
* **The Concept:** Each cloud system uses different protocols and different APIs (Application Programming Interfaces). Because of this, it may not be possible to seamlessly run applications between different cloud-based systems.


* **Simple Explanation:** Amazon (AWS), Microsoft (Azure), and Google (GCP) all built their clouds differently. They don't speak the exact same technical language. If you build your company's software to work perfectly on Amazon's cloud, you can't just copy and paste it over to Microsoft's cloud if you find a cheaper price there.
* **Real-Life Example:** It is like buying a video game for a Sony PlayStation. If you later decide to buy a Microsoft Xbox, you can't just put your PlayStation disc into the Xbox. The systems do the exact same job, but they speak different languages.


### **3. Forced Adaptation (Proprietary Systems)**
* **The Concept:** Cloud providers often build custom, proprietary tools. For instance, Amazon created its own database system (which doesn't use the standard SQL 92) and its own workflow systems. Therefore, your normal applications will have to be adapted to execute on these specific platforms.


* **Simple Explanation:** When you run servers in your own office, you usually build software using universally standard tools. But when you move to the cloud, providers want you to use *their* custom-built tools because they run faster on their specific hardware. To make your existing software work, your programmers have to spend a lot of time rewriting the code to fit the cloud provider's unique rules.
* **Real-Life Example:** Imagine moving your business to a new country that uses a completely different alphabet and currency. You can still do business there, but you have to spend a lot of time and money translating your signs, menus, and price tags before you can open your doors.

## Data Security risk in the cloud
- Data security
- Data privacy
- Data loss
- Account hijacking
- Insecure APIs
- Insider threats
These problems occur because data and services are stored remotely and accessed through the internet.

## What is the Service Level Agreement (SLA)?
SLA is a formal contract between a cloud service provider (CSP) and the customer that defines that level of service expected from the provider.

### Why is SLA used?
1) Clarity of Expectations
2) Reliability Assurance
3) Accountability
4) Customer Trust
5) Business Continuity
  
### Key Components of an SLA
- Service Availability (Uptime)
- Performance Metrics (response times or applications, speed of data transfer, or API responsiveness)
- Support and Response Times
- Data Security and Privacy (encryption, backups, and compliance standards)
- Data Backup and Recovery
- Penalies for Non-Compliance
- Termination Terms 