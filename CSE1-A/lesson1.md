# Week 1
## Background
- Target
  * Define cloud computing in your own words and explain why "the cloud" is a metaphor.
  * Distinguish the five cloud deployment models and identify which one a given business needs.
  * Name the five defining characteristics of cloud computing and recognize them in read services.
  > "The cloud" is not a place. IT's a metaphor for the internet — specifically, for sharing data or running applications on someone else's computer infrastructure (AWS, Azure, Google Cloud) instead of your own.
  
  > The term first appeared in a 1996 Compaq internal document; entered the mainstream in 2006 with AWS EC2.

## What is Cloud Computing?
- Renting computing power instead of owning it
  * Cloud computing
    + The dilivery of computing services — servers, storage, databases, networking, software and analytics — over the internet, instead of from hardware you own on-site.
    + Insteaf of buying and maintaining physical servers on-premises, you access computing resources over the internet and pay only for what you use — on demand, like a utility bill.
  * On-premises vs Cloud
    | On-Premises | Cloud |
    |---|---|
    | You own & maintain the hardware | Provider owns & maintains it
    | Large upfront capital cost | Pay-as-you-go operating cost
    | Fixed-capacity — hard to scale fast | Scales up or down on demand
    | You handle updates & security patches | Provider handles the insfrastructure layer
- One shared pool, accessed by everyone
  * Cloud service models are built on sharing on-demand computing resources over the internet. Companies and individuals pay to access a virtual pool of compute, storage, and networking that lives on remote servers owned and managed by a provides — not by them (individuals or companies).
  ```
    Resources Provided                                    Who Accesses It
    |-----------------|                                 |-----------------|
    |     Compute     |--\                           /--|    Company A    |
    |-----------------|   \                         /   |-----------------|
    |     Storage     |----\ |———————————————————| /----|    Company B    |
    |-----------------|    |-| Shared Cloud Pool |-|    |-----------------|
    |   Networking    |----/ |———————————————————| \----| Individual User |
    |-----------------|   /                         \   |-----------------|
    |    Databases    |--/                           \--|     Startup     |
    |-----------------|                                 |-----------------|
  ```
## Cloud Deplyment Types
- Five deployment models, one decision: who owns the infrastructure?
  * Overview:
    1. Public
    + Owned by a third-party provider; resources shared across many custormers — or "tenants".
    2. Private
    + Dedicated to a single organization, on-premises, or hosted, for control and compliance.
    3. Hybrid
    + Combines public and private cloud infrastructures, sharing data and apps between the two.
    4. Community
    + Shared by several organizations with a common purpose, like reseach or healthcare.
    5. Multicloud
    + Multiple public/private ckiyds from different vendors, used side by side.
  * Public 
    > Shared infrastructure, third-party owned.
    + Definition:
      - Owned and operated by third-party providers (e.g. AWS, Microsoft Azure, Google Cloud). 
      - Resources are shared among multiple customers or "tenants", and billed on a pay-as-you-go bases.
      - Its defining trait is multitenancy; the same physical infrastructure serves many users, each in an isolated virtual environment
    + Example:
      - Netflix
        * Provider: Amazon Web Services (AWS)
        * Streams to multiple of users worldwide; scales instantky with demand and runs its recommendation analysis on AWS.
      - Airbnb
        * Provider: Amazon Web Services (AWS)
        * Uses cloud elasticity to absord traffic spikes during peak travel seasons, without owning extra servers.
      - Spotify
        * Provider: Google Cloud Platform (GCP)
        * Analyzes listening data in real time to personalize playlists and manage its full music catalog.
    + Pros and Cons
      | Pros | Cons |
      | High scalable on demand | Less direct control over infrastructure |
      | Cost-efficient — no hardware to buy | Data sites alongside other tenant' data |
      | Zero infrastructure maintenance | Security concers for sensitive workloads |
  * Private Cloud
    > Dedicated infrastructure, single operation.
    + Definition:
      - Infrastructure maintained on a private network for one organization only, offering greater control, security, and customization.
      - Private clouds can be hosted on-premises or by a third parte and provire dynamic provisioning of resources exclusively for that organization — often to meet strict regulatory or compliance requirements.
    + Examples:
      - Internet Business Machines (IBM)
        * Provider: IBM Cloud (Private)
        * Runs critical enterprise applications with a focus on security and compliance, keeping full infrastructure control while still offering cloud services to clients.
      - Typical Users
        * Provider: In-house or self-hosted
        * Banks, government agencies, and hospitals — organizations where regulation or sensitivity rules out shared infrastructure.
    * Pros and Cons
      | Pros | Cons |
      |---|---|
      | High security and data control | Expensive to buld and run |
      | Fully customizatble to organizational needs | Requires dedicated maintenance staff |
      | Easier regulatory compliance | Harder to scale than public cloud |
  * Hybrid Cloud
    > Public + private, working together.
    + Definition:
      - A combination of public and private clouds that allows data and applications to move between them.
      - Hybrid cloud exists because of private deployments alone struggle to scale on demand for peak loads — so organizations keep sensitive workloads private and burst everything else onto public infrastructure when needed.
      > Stores sensitive data in a private cloud, while using public cloud capacity for less-sensitive, high-volume tasks.
    + Example:
      - Dropbox
        * Provider: AWS + in-house private cloud
        * Started fully on AWS, then shifted to hybrid — private infrastructure for data storage, AWS for large-scale compute — for cost savings and flexibility.
    + Pros and Cons
      | Pros | Cons |
      |---|---|
      | Flexible — best of both models | Complex to configure and manage |
      | Cost-effective for mixed workloads | Requires integration between environments |
      | Scales for peak demand without public exposure | |
  * Community Cloud
    > Shared by organizations with a common mission.
    + Definition:
      - Infrastructure shared by several organizations that have a common purpose — sure as a group of universities, hospitals, or government agencies.
      - It may be managed internally by the participating members or by a third-party, with costs, reponsibilities, and security protocols shared across the community.
      > A consortium of institutions with overlapping compliace needs pools resources instead of each building separate infrastructure.
    + Example:
      - Cloud4EU
        * Provider: Shared infrastructure (EU)
        * European universities and government-funded reseach labs build a shared cloud to support scientific research and data collaboration — governed jointly, not owned by one institution.
    + Pros and Cons
      | Pros | Cons |
      |---|---|
      | Shared cost across all members | Governance can be slow with many stakeholders |
      | Tailored to a specific sector's compliace needs | Still more expensive than public cloud | 
      | More collaborative than a single private cloud | Limited to members of the community |
  * Multicloud
    > Multiple providers, best tool for each job.
    + Definition:
      - The use of multiple cloud computing services from different providers, letting an organization pick the best-suited service for each need and avoid vendor lock-in.
      - Unlike hybrid cloud — which links public and private — multicloud simply means running on several public/private clouds that aren't necessarily connected to each other.
      > Combines Internet as a Service (IaaS) from one vendor (e.g. AWS + Azure) with Platform as a Service (PaaS) or Software as a Service (SaaS) from another (e.g. Salesforce + Microsoft 265) to match each workload to its best platform.
    + Example:
      - Provider: AWS, Microsoft Azure, Google Cloud
      - Runs several banking systems and portals across several providers, letting teams modernize and unlock data across an optimized, multi-vendor cloud ecosystems.
    + Pros and Cons
      | Pros | Cons |
      |---|---|
      | Avoids vendor lock-in | Most complex model to manage |
      | Leverages each provider's strengths | Requires skills across multiple platforms |
      | Improves resilience if one provider has an outage| |
- Side by side: choosing the right model
    | Type | Owned by | Best for | Example |
    | --- | --- | --- | --- |
    | Public | Third-party provider | Startups, variable-traffic apps | Netflix (AWS) |
    | Private | Single organization | Regulated, sensitive workloads | IBM (IBM Cloud) |
    | Hybrid | Shared (public + private) | Mixed sensitivity workloads | Dropbox (AWS + own) |
    | Community | Group of organizations | Shared-mission sectors (research, health) | CLOUD4EU |
    | Multicloud | Several vendors at once | Avoiding lock-in, best-of-breed tools | JPMorage Chase |
## Characteristics of Cloud Computing
- The five traits every true cloud service has:
  1. On-Demand Self-Service
    + Users provision computing resources automatically, whenever they need them — no, homan at the provider required.
  2. Broad Network Access
    + Users are available over the network through standard mechanisms, reachable from phones, laptops, and tablets alike.
  3. Resource Pooling
    + A provider's resources serve multiple customers from a shared pool, dynamically assigned and resasigned by demand.
  4. Rapid Elasticity
    + Capacity can scale up or down quickly — often automatically — to match real-time demand.
  5. Measure Service
    + Usage is metered automatically, so systems optimize systems and users pay only for what they actually use.