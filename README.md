# AWS Cloud Foundation Basic — Level 1
----
**Duration:** 2 months (8 weeks)  
**Schedule:** 3 sessions per week (24 sessions total)  
**Level:** Beginner  
**Prerequisite:** Basic computer literacy  
**Capstone:** Deploy a live static website on Amazon S3  
**Next step:** Level 2 — Intermediate AWS Cloud Engineering
---
## Course promise
### This course takes learners from zero cloud experience to confidently navigating AWS, explaining core cloud concepts, applying basic security practices, creating introductory compute/network/storage resources, monitoring costs, and publishing a simple website.
### It is a practical foundation course. It is **not** a production cloud architecture or AWS certification-preparation guarantee.
---
## Who should take it?

- Complete beginners curious about cloud computing
- IT support staff who want to move into cloud
- Career changers beginning an AWS/cloud journey
- Learners with basic computer and internet skills
---
## Learning outcomes
By the end, learners should be able to:

1. Explain cloud computing, shared responsibility, regions, Availability Zones and common cloud service models.
2. Navigate the AWS Management Console and identify key service categories.
3. Secure an AWS account using MFA, IAM users/roles and least-privilege principles.
4. Explain the purpose of VPCs, subnets, route tables, internet gateways and security groups.
5. Launch, connect to, inspect and safely terminate a basic EC2 instance.
6. Explain S3 buckets, objects, storage classes and introductory database concepts.
7. Use CloudWatch basics, AWS Budgets and cost-aware resource cleanup.
8. Publish and verify a simple static website using Amazon S3 website hosting.
9. Document practical work with screenshots, short explanations and diagrams.
---
## Weekly rhythm

| Day | Learning mode | Typical activities |
|---|---|---|
| Day 1 | Understand | Concepts, vocabulary, instructor demonstration and discussion |
| Day 2 | Guided lab | Instructor-led AWS console practice |
| Day 3 | Apply | Independent task, troubleshooting, project checkpoint and review |

Recommended session length: 2–3 hours.
---
## Repository map

```text
.
├── README.md
├── INTRODUCTION.md
├── COURSE_OUTLINE.md
├── CURRICULUM.md
├── lessons/
│   ├── week-01-cloud-fundamentals/
│   ├── week-02-aws-account-and-iam/
│   ├── week-03-aws-global-infrastructure/
│   ├── week-04-networking-fundamentals/
│   ├── week-05-compute-services/
│   ├── week-06-storage-and-databases/
│   ├── week-07-security-and-monitoring/
│   └── week-08-website-deployment/
├── assignments/
│   ├── weekly-assignments.md
│   └── assessment-rubric.md
├── projects/
│   ├── weekly-projects.md
│   └── final-capstone.md
└── instructors-guide/
    ├── teaching-guide.md
    ├── lab-instructions.md
    ├── marking-guide.md
    └── troubleshooting.md
```
---
## Before the first lab

- Each learner should have a computer, reliable internet access and a modern browser.
- Create or use an AWS account only with the account owner's informed permission.
- Add MFA to the root user and do not use root for everyday work.
- Set an AWS Budget and billing alerts before creating resources.
- Never share passwords, access keys, secret keys, payment details or unredacted billing screenshots.
- Use a dedicated learning account where possible. Do not practise in an employer's production account.
- Check current AWS pricing and Free Tier eligibility before every lab. Free Tier eligibility and offers can change; **do not promise that every activity is free**.
- Delete or stop resources after labs. Stopping an EC2 instance does not necessarily remove every charge (for example, attached storage or allocated public IPv4 addresses may still incur charges).
---
## Safety rules

1. Never publish credentials in GitHub, chat, screenshots or class submissions.
2. Never disable security controls simply to make a lab work.
3. Do not place personal or confidential information in public S3 buckets.
4. Make public access intentional, limited to the website's public files, and remove it after the lab if the site is no longer needed.
5. Use only instructor-approved regions and resource sizes.
6. Verify the account, region and resource name before pressing **Create**, **Delete** or **Terminate**.
7. Ask the instructor before creating anything that could incur significant cost.

## Assessment

- Weekly practical tasks and short reflections: 30%
- Weekly project evidence: 20%
- Participation, lab discipline and troubleshooting: 10%
- Final capstone website and explanation: 40%

Suggested pass mark: 60%. 
---
## How to use this repository

Learners should work through the weekly lesson folders in order. For each practical activity, submit:
- What you were asked to build
- A simple diagram or list of steps
- Screenshots with sensitive information hidden
- What worked and what did not
- How you cleaned up the resources
---
## Suggested GitHub setup

Create a public or private repository named `aws-cloud-foundation-basic`. Upload the contents of this folder to the repository root. Use GitHub Issues for questions and weekly project tracking. Do not upload AWS credentials, account IDs if your organisation treats them as confidential, or personal billing information.

## Disclaimer

AWS console labels, pricing, service availability and account onboarding flows may change. The instructor should verify current AWS documentation and pricing before delivering the course. This material is an educational foundation, not a substitute for AWS documentation or production security review.
