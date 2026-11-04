# Eight-Week Curriculum — 24 Sessions

## Week 1 — Cloud Computing Fundamentals

**Goal:** Explain cloud computing in everyday language and identify why organisations use it.

### Day 1 — What is cloud computing?
- Define cloud computing and on-demand resources.
- Compare on-premises infrastructure with cloud services.
- Discuss servers, storage, networks and applications.
- Explain scalability, elasticity, availability and pay-as-you-go.
- Activity: identify cloud services learners already use.

### Day 2 — Cloud deployment and service models
- Public, private and hybrid cloud.
- IaaS, PaaS and SaaS.
- Responsibility differences across service models.
- Examples: virtual servers, managed platforms and webmail.
- Activity: classify familiar technology products by service model.

### Day 3 — Benefits, limitations and architecture thinking
- Benefits: agility, global reach, flexible capacity and managed services.
- Trade-offs: cost control, outages, security configuration, vendor dependency and internet access.
- Introduce a simple architecture diagram.
- Project: sketch a small organisation's website and identify its compute, storage and network needs.

**Deliverable:** One-page cloud explanation and labelled diagram.

## Week 2 — AWS Account, Console and Identity

**Goal:** Navigate AWS safely and explain how identities and permissions work.

### Day 1 — AWS and the Management Console
- What AWS provides and how services are grouped.
- Account, console, region selector and search.
- Service categories: compute, storage, networking, database, security and monitoring.
- Demonstration: navigate the console without creating resources.

### Day 2 — Account safety and root user
- Root user versus everyday identities.
- Multi-factor authentication (MFA).
- Billing contact and account security basics.
- Why root should not be used for routine tasks.
- Lab: inspect root security settings with instructor guidance; enable MFA where authorised.

### Day 3 — IAM foundations
- Users, groups, roles and policies.
- Authentication versus authorisation.
- Least privilege and permission boundaries as a concept.
- Lab: create a limited training identity or role only if the training account setup permits it; test access and remove temporary identities.
- Never create or distribute long-lived access keys for this beginner console course.

**Deliverable:** Account safety checklist and IAM relationship diagram.

## Week 3 — AWS Global Infrastructure

**Goal:** Explain where AWS resources run and why location matters.

### Day 1 — Regions
- What a Region is.
- Choosing a Region: latency, service availability, legal/data location needs and cost.
- Region selection in the console.
- Activity: compare two Regions using AWS's current public information.

### Day 2 — Availability Zones
- What an Availability Zone (AZ) is.
- Why AZs support fault isolation and resilience.
- Region versus AZ.
- Understand that not every service is configured or scoped in the same way.
- Activity: draw one Region containing multiple AZs.

### Day 3 — Edge locations and service scope
- Edge locations and content delivery concept.
- Global, regional and zonal resource examples.
- How to verify the selected Region before creating a resource.
- Project: prepare a Region and AZ fact card for a hypothetical website.

**Deliverable:** Region/AZ diagram and a short Region selection justification.

## Week 4 — Networking Fundamentals

**Goal:** Understand the basic network components used by AWS resources.

### Day 1 — Networking vocabulary
- Network, IP address, public and private IP.
- IPv4 address and CIDR notation at an introductory level.
- DNS and domain names.
- Ports and protocols: HTTP 80, HTTPS 443, SSH 22 (conceptual; SSH must be tightly restricted).
- Activity: trace what happens when a browser opens a website.

### Day 2 — Amazon VPC and subnets
- What a VPC is: a logically isolated network.
- CIDR range and subnet.
- Public versus private subnet (based on routing, not simply a label).
- Route tables and routes.
- Draw a simple VPC with one public subnet.

### Day 3 — Internet access and traffic controls
- Internet gateway.
- Route to an internet gateway.
- Security groups as stateful virtual firewalls.
- Network ACLs as stateless subnet-level controls (concept only).
- Lab: inspect the default VPC and its components; do not modify shared/default networking without approval.
- Project: draw and explain a basic VPC network.

**Deliverable:** Labelled network diagram and five networking definitions.

## Week 5 — Compute with Amazon EC2

**Goal:** Explain virtual machines and perform a safe introductory EC2 lab.

### Day 1 — Compute concepts
- What a server does.
- Physical server versus virtual machine.
- What EC2 provides.
- Instance families and sizes at a high level.
- AMI, instance type, key pair, storage and security group.
- Cost awareness: instance runtime and associated resources.

### Day 2 — Launch an EC2 instance
- Review the lab plan and expected costs.
- Select an instructor-approved Region and small eligible instance type.
- Choose an approved AMI.
- Configure storage and security group.
- Avoid opening SSH/RDP to the whole internet. Use approved access methods and instructor-controlled source IPs.
- Launch and inspect instance state and status checks.

### Day 3 — Connect, test and clean up
- Connect using the approved method (EC2 Instance Connect or SSH where supported).
- Identify basic Linux commands: `pwd`, `ls`, `whoami`, `sudo`, `systemctl` (explain only), `ip`.
- Optional instructor demo: install a simple web server and display a test page.
- Stop or terminate the instance as instructed; inspect attached volumes and any other billable resources.
- Project: demonstrate a basic EC2 instance and explain its security group.

**Deliverable:** EC2 lab report with redacted screenshots and cleanup confirmation.

## Week 6 — Storage and Database Fundamentals

**Goal:** Explain object storage and distinguish storage from databases.

### Day 1 — Amazon S3
- Object storage, buckets and objects.
- Bucket names and Region considerations.
- Upload, download, folders/prefixes and metadata.
- Common uses: website assets, backups and documents.
- Storage classes introduced conceptually.

### Day 2 — S3 access and data protection
- Bucket policies and IAM permissions at a high level.
- Block Public Access and why it should normally remain enabled.
- Encryption at rest concept.
- Versioning and lifecycle rules concept.
- Lab: create a private bucket, upload sample files, test access and delete the lab data.

### Day 3 — Database foundations and RDS
- Files versus structured records.
- Relational databases, tables, rows and columns.
- What Amazon RDS manages.
- Database availability, backups and credentials.
- Why a database should not be exposed publicly for a beginner demo.
- Project: create a private S3 portfolio-assets bucket and document its access design. Do not create RDS unless the instructor has approved the cost.

**Deliverable:** S3 storage exercise and short comparison of S3 versus a relational database.

## Week 7 — Security, Monitoring and Cost Awareness

**Goal:** Apply beginner security habits and understand how to observe and control cloud usage.

### Day 1 — Cloud security foundations
- Shared Responsibility Model.
- AWS security of the cloud versus customer security in the cloud.
- MFA, least privilege and credential hygiene.
- Encryption and secure data handling.
- Public exposure risks.
- Activity: identify security mistakes in a sample cloud setup.

### Day 2 — Monitoring with CloudWatch
- What monitoring is and why it matters.
- Metrics, logs and alarms.
- EC2 status checks and basic metrics.
- CloudWatch dashboards introduced.
- Lab: view available metrics for a lab resource; create an alarm only if approved and explain possible alarm costs.

### Day 3 — Cost management and operational hygiene
- Billing dashboard and cost categories.
- AWS Budgets and budget alerts.
- Cost Explorer concept.
- Tags for ownership and environment.
- Resource inventory and cleanup checklist.
- Project: perform a security and cost review of a sample AWS account design.

**Deliverable:** One-page security, monitoring and cost checklist.

## Week 8 — Deploy a Website and Course Review

**Goal:** Publish and explain a simple static website using Amazon S3.

### Day 1 — Prepare the website
- Static versus dynamic websites.
- HTML, CSS, JavaScript and website assets at a basic level.
- Website files: `index.html` and optional `error.html`.
- How a browser requests a website.
- Plan bucket name, Region, files and access requirements.

### Day 2 — Deploy with Amazon S3 static website hosting
- Create a dedicated capstone bucket.
- Upload the approved static website files.
- Configure static website hosting.
- Explain public-read access required for the basic S3 website endpoint and the associated risks.
- Apply only the narrow, instructor-reviewed bucket policy required for the lab.
- Keep Block Public Access enabled except for the specific, deliberate setting change required by the exercise.
- Test the website endpoint.
- Note: the S3 website endpoint does not itself provide HTTPS. Custom domains and HTTPS/CDN design are topics for later training.

### Day 3 — Test, present and clean up
- Test page loading and links.
- Check browser behaviour and troubleshoot common errors.
- Explain the architecture and security choices.
- Present the capstone.
- Remove public access and delete lab resources if the site is not intended to remain live.
- Course review and next-step guidance.

**Deliverable:** Working website URL during assessment, source files, architecture diagram, demonstration and cleanup evidence.

---

## Suggested session lesson template

For every session, the following must be recorded:
- Session title and learning objectives
- New vocabulary
- Explanation and real-world example
- Instructor demonstrations
- Students' practical task
- Questions/check for understanding
- Homework or reflection
- Cost/security reminder
- Cleanup confirmation
