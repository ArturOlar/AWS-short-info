### EC2 instances types

Instance types (https://aws.amazon.com/ec2/instance-types/):
- general purpose
- compute optimized
- memory optimized
- accelerated computing
- storage optimized
- HPC optimized
- instance features
- measuring instance performance

AWS has the following name convention. For example we have **m5.2xlarge**
- m - instance class (in this case it's general purpose)
- 5 - generation of the instance (AWS improves them over the time)
- 2xlarge - size within the instance class

---

#### General Purpose

**General Purpose** instances starts from letter **M** and **T**, for example: **M7g**, **M6g**, **T3**, etc.

- great for a diversity of workloads such as web servers or code repositories
- good balance between:
    - compute
    - memory
    - networking

---

#### EC2 Instance Types – Compute Optimized

**Compute optimized** instances starts from letter **C**, for example: **C7g**, **C6g**, **C6a**, etc.

- great for compute-intensive tasks that require high performance processors:
    - Batch processing workloads
    - Media transcoding
    - High performance web servers
    - High performance computing (HPC)
    - Scientific modeling & machine learning
    - Dedicated gaming servers

---

#### EC2 InstanceTypes – Memory Optimized

**Memory optimized** instances starts from letter **R**, **X**, **Z** and **High Memory**, for example: **R7g**, **R6g**, **x2iedn**, **z1d** etc.

- fast performance for workloads that process large data sets in memory (RAM)
- use cases:
    - High performance, relational/non-relational databases
    - Distributed web scale cache stores
    - In-memory databases optimized for BI (business intelligence)
    - Applications performing real-time processing of big unstructured data

---

#### EC2 InstanceTypes – Storage Optimized

**Storage optimized** instances starts from letter **I**, **D**, **H**, for example: **I4g**, **D3**, etc.

- great for storage-intensive tasks that require high, sequential read and write access to large data sets on local storage
- use cases:
    - High frequency online transaction processing (OLTP) systems
    - Relational & NoSQL databases
    - Cache for in-memory databases (for example, Redis)
    - Data warehousing applications
    - Distributed file systems

---

Website to compare all EC2 instances - https://instances.vantage.sh/`
