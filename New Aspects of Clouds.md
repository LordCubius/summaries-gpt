Summary of the Transcript on Cloud Computing

1. On-Demand Access in Cloud Computing

    Cloud services allow users to pay only for what they use, rather than purchasing resources upfront.
    Example: You pay for computing power (CPU hours) or storage (per gigabyte per month) instead of buying hardware. AWS EC2 and Microsoft Azure are popular providers.
    This model is akin to renting a cab (on-demand) rather than renting a car (owning hardware or a datacenter).

2. Cloud Service Classifications ("aaS")

    Hardware as a Service (HaaS): Provides raw hardware access, where users manage the machines themselves. However, it is less common due to security risks when granting untrusted users root access to physical machines.

    Infrastructure as a Service (IaaS): Provides virtualized computing resources (e.g., VMs) where users install their own OS and manage machines. Major platforms like AWS and Azure offer IaaS, which is popular in public clouds. IaaS often subsumes HaaS in practice.

    Platform as a Service (PaaS): Offers a more integrated service than IaaS, where users write code without worrying about managing VMs or infrastructure. Example: Google App Engine.

    Software as a Service (SaaS): Provides ready-to-use software applications on demand. Examples include Google Docs, Microsoft Office 365, and other web-based applications. SaaS may also include Service-Oriented Architectures (SOA).

3. Data-Intensive vs. Computation-Intensive Computing

    Traditional distributed systems were computation-intensive, focusing on high-performance computing tasks (e.g., weather modeling). In contrast, modern cloud systems focus on data-intensive computing, processing large volumes of data (e.g., petabytes, exabytes) rather than complex computations.
    Shift in focus: From computation to managing and processing large datasets, where proximity between data and compute resources is crucial.
    Metrics of resource utilization: While CPU utilization was previously the key metric for computation-intensive tasks, now I/O (disk and network I/O) is a critical factor, especially in data-heavy clouds.

4. New Cloud Programming Paradigms

    Cloud programming paradigms focus on handling large-scale data, with a major example being MapReduce, which processes huge datasets by dividing the workload across many machines.
        MapReduce was popularized by Google and later implemented in Apache Hadoop, which was open-sourced by Yahoo.
        Amazon Elastic MapReduce (EMR) offers a pay-as-you-go service for MapReduce tasks.
    Notable use cases:
        Google uses MapReduce to index data for its search engine, processing 50 petabytes/month with 200,000 jobs in 2006.
        Yahoo uses MapReduce for web map applications, processing 280 terabytes in 73 hours with 2,500 nodes.
        Facebook uses Hadoop and Hive (a data warehouse built on top of Hadoop) for large-scale data processing.
        Other examples: eHarmony uses MapReduce for matching users in overnight runs.
    Data Storage and Querying: In addition to processing data, new cloud systems focus on efficient storage and querying.
        Traditional relational databases like MySQL are still in use, but NoSQL and Key-Value Stores have become dominant due to their speed and scalability in cloud environments.

This lecture emphasizes the shift towards data-intensive computing in cloud environments, the on-demand access pricing model, and the evolution of cloud services from infrastructure (IaaS) to more abstracted services like PaaS and SaaS. It also introduces the MapReduce paradigm and other cloud programming models, which are essential for large-scale data processing.