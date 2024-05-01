# Interview approach

This are guidelines I follow when I interview candidates for an Engineering role.
I have been interviewed by many companies and I have been a hiring manager for some time, I have seen and experienced first hand a lot of different approaches to the interview process.

This is a collection of unsorted questions that purposefully have no answers. The idea is to use this as a reference for your own interview process.

# Intro

- How are you doing/weather, something nice to break the ice and make the candidate feel comfortable
- Tell me about your engineering journey, how did you get into engineering?
- What do you like about this job?
- What are you looking for in your next role?
- What is your favorite programming language and why?
- What is the best piece of code you have ever written? And the worst?
- Do you hate PHP? (I do)
- Are you nervous? (I am)

# General 

## Git

- What is the difference between a remote branch and a local branch?
- How can I delete a remote branch? Please give the command
- What’s a tag and how is it used?
- What’s a hook? Make an example of its use.
- What’s a submodule and when should it be used?
- How can I rollback the last commit I made on my local branch?
- Rebase vs merge, explain the difference and when to use one or the other

## Network

- How does the TCP/IP protocol work?
- What’s a DNS and how does that work?
- What is a VPN?
- What is a NAT tunnel?
- How does DHCP work?
- What is a firewall? What is a WAF?
- How would you block a specific IP address from accessing a service?
- What is a proxy? What is a reverse proxy? What is a forward proxy?
- How does a load balancer work?
- Do you know any Load Balancing algorithms? Explain them (e.g. Round Robin, Least Connections, etc.)

## Linux and Virtualization

- What is Linux and what makes it different from other operating systems?
- What is a directory?
- What’s "the kernel"?
- How can you install software on a Linux system and what are the common package managers used in Linux?
- What’s the command for changing the permission of a file? Give an example
- What’s the command for changing the ownership of a file? Give an example
- What’s a command for killing a process given its PID? Give an example
- What’s a command to list all the processes running? Give an example
- What’s the command, named after a protocol, to connect to a remote server in Linux? Give an example
- What’s a service in Linux?
- How does SELinux work?
- What does it happen when you launch `$?` in bash?
- What is a virtual machine (VM) and how does it work?
- What’s a hypervisor software?

# DevOps, SRE and Platform Engineering

## CI/CD

- What’s CI/CD?
- Explain the phases of CI/CD
- Have you ever used GitHub actions? How does it work?
- Have you ever used GitLab? How does it differ from GitHub?

## Docker and Containerization

- What’s the difference between a virtual machine and a container runtime?
- How does containerization work?
- Is Docker the only way to create a container?
- What is the purpose and power of an image?
- What is the registry and how is it used in containerization?
- What’s a Dockerfile?
- What is the first line of a Dockerfile?
- How do you attach a volume in a Docker container?
- How do you manage or orchestrate multiple containers?
- What’s the purpose of Docker Compose?
- Best practice for building a good Dockerfile
- Why too many lines are bad for a Dockerfile?

## Cloud

- What is cloud computing?
- Define public, hybrid, and private cloud and give a use case for each
- What is serverless?
- Is I say edge computing, what do I mean?
- List some CNCF (Cloud Native Computing Foundation) graduated projects or projects you like

## Site Reliability Engineering

- What is a receiver in an alert manager?
- What happens when you execute a `curl` command on a Prometheus exporter endpoint?
- Give me an example of an OpenMetrics payload
- What is a Service Level Objective (SLO)?
- What is a Service Level Indicator (SLI)?
- What is a Service Level Agreement (SLA)?
- If I say "Error Budget", what do I mean? SLA is 99.9%, what is the error budget?

## Terraform and Infrastructure as Code

- What is Infrastructure as Code and why is it important in modern cloud development?
- Explain the following commands: terraform init, terraform plan, terraform apply
- What is the purpose of the Terraform state file?
- What is Terraform's remote state?
- Where should it be stored, for example, in AWS as a cloud provider?
- What is a Terraform provider and what’s the difference between a provider and a resource?
- What is the way of reusing Terraform templates?
- How can you use Terraform variables?
- What major cloud provider can Terraform work with?
- How does Terraform handle updates to existing resources?
- How does Terraform handle dependencies between resources?

## Kubernetes, Helm, and Container Orchestration

- What is Kubernetes, and what are some of its main features and benefits?
- What are the components of a Kubernetes cluster, and how do they interact with each other?
- How can you interact with Kubernetes API?
- Explain these commands: k create, k get, k describe, k delete, k apply, k logs, k exec, scale, rollout
- How do you create a Kubernetes deployment, and what are some best practices to follow when defining deployments?
- What is an ImagePullPolicy and what values can this parameter hold?
- What is a Kubernetes port forward? Why do you use that? What’s the command to perform that?
- NodePort vs LoadBalancer?
- What is the role of the Scheduler?
- Explain node affinity, node taints, node selectors, and pod priority.
- What are Kubernetes pods, and how do they relate to containers?
- Explain the Pod lifecycle
- What is the CrashLoopBackOff state?
- Explain the following command 
```
kubectl run nginx --image=nginx:latest --port=80 --env="ENV_VAR=value" --labels="app=nginx" --
limits="cpu=500m,memory=256Mi" --requests="cpu=250m,memory=128Mi" --dry-run=client -o yaml > nginx.yaml
```
- What’s the difference between resource request and resource limit in Kubernetes?
- When is a Pod evicted?
- How does Kubernetes health checks work?
- What is a livenessProbe ?
- What is a readinessProbe ?
- What is a startupProbe ?
- How many kinds of probe types are there?
- NodeAffinity vs PodAffinity
- What is the POD disruption budget?
- What is a Kubernetes volume?
- How is a Kubernetes volume different from a container's file system?
- What are some types of Kubernetes volumes?
- How do you define a Kubernetes volume in a Pod's YAML configuration?
- How do you mount a Kubernetes volume to a container?
- Can multiple containers in a Pod share the same volume?
- What is a Persistent Volume (PV) in Kubernetes?
- How do you define a Persistent Volume in Kubernetes?
- How do you claim a Persistent Volume in Kubernetes (PVC)?
- How do you use a Persistent Volume in a Pod?
- What is a StorageClass and how does that work?
- What are the benefits of StorageClass?
- What is a Kubernetes namespace, and how can it be used to manage resources in a multi-tenant environment?
- What are Kubernetes Services, and how do they enable application discovery and load balancing?
- What is an Ingress and how does it work?
- What is a Kubernetes Controller and how does it work?
- Explain the difference between ReplicaSet controller, Deployment controller, StatefulSet controller, and DaemonSet controller
- What is a secret, and how can it be used to manage sensitive information like passwords and API keys?
- How do you scale a Kubernetes deployment, and what factors should you consider when determining the optimal number of replicas?
- Also, what metrics exist (natively) that can trigger a new pod?
- What kind of autoscaling is Kubernetes capable of?
- What is HPA and how does it work?
- What is Cluster Autoscaling and how does it work?
- What is a ConfigMap?
- What’s a Kubernetes Operator?
- Explain RBAC - Role Based Access Control
- What is the difference between Role and RoleBinding?
- Role vs ClusterRole, explain the difference
- What are some best practices for monitoring and logging Kubernetes clusters and applications running on them?
- Do you have any experience with Grafana+Prometheus, New Relic, Datadog, Dynatrace, or other similar products?
- How would you decide to separate Kubernetes clusters in an organisation? In what conditions would you have a single cluster?
- How do you manage multi-tenancy on Kubernetes in general and in terms of billing?

## Helm

- What is Helm?
- Explain helm create, helm package, and helm install commands
- What does this `replicas: {{ .Values.replicaCount }}` mean?
- How does helm templating work?
- What is Jinja?
- How can you see the story of the releases in helm?
- Describe how to perform a go to the previous version in helm

## Platform Engineering

- What is Platform Engineering?
- What is the difference between DevOps, SRE and Platform Engineering?
- What is the tooling you use for Platform Engineering?
- Should I go Platform Engineering if I have one product and one team?

See: https://github.com/mbianchidev/platform-engineering-roadmap

## OpenShift

- Do you have any experience with OpenShift Container Platform?
- What is OpenShift?

## Ansible

- What is the difference between Playbook and Role?
- How do you debug a Playbook?
- How would you use Ansible to automate the deployment of a web application?

## AWS

- Define these AWS Services: EC2, S3, Route 53, Lambda, IAM
- What kind of different Load Balancers does AWS offer?
- Define these networking resources in AWS: VPC, ACL, NACL
- What’s the difference between EKS, ECS, and ECR?
- What is CloudFormation and how does it work?

## Azure

- How would you deploy a web application to Azure App Service?
- Can you explain the difference between Azure Virtual Machines and Azure Kubernetes Service (AKS), and when you might choose one over the other?
- How do you configure Azure Active Directory for use in a single-sign-on (SSO) scenario?

# Software Engineering 

## Backend

- Explain SOLID principles
- Do you know any design pattern? Pick your favorite one and explain it (e.g. Decorator, Facade, Observer)
- What is a RESTful API?
- What’s the difference between 2xx, 4xx, and 5xx error codes?
- What is a Microservice architecture and how it differs from a monolithic one?
- Explain OOP
- Explain functional programming
- Explain what is a Queue in programming and make some examples of different types of Queues (LIFO, FIFO...)
- How do you handle errors in your code?
- What is a distributed system?
- Have you ever used a message broker? What is it and how does it work?
- What is a cache? What is it used for?
- Why is redis so fast?

## Microservices

- Why should I use separate data storage for each microservice?
- What does it meen to keep code at a similar level of maturity?
- What entails to separate build for each microservice?
- Should I assign each microservice multiple responsibility?
- Are containers useful in microservices?
- Stateless microservices seem to be bad. Can I go stateful with microservices? 
- Should I Adopt DDD (Domain Driven Design)?
- Orchestrating microservices is not easy. What are the options?

## Backend Engineering Scenarios

- What’s canary deployment?
- What if I have two deployments 1.0 (production, stable) and 1.1 (test, maybe stable) and I want to test 1.1 with production traffic, without using the canary deployment technique, what alternatives have I got?
- What if I have a log file that multiple processes write to, how can I make sure that the log file is not corrupted?

## Database

- What kind of databases do you know? Pick one and convince me it's the best kind of db ever for my application (e.g. In memory, time series, document, vectorial)
- Explain DB data structures (e.g. B-Tree, Hash Table, LSM tree etc.)
- What is a query execution plan? Can you "explain" it?
- What is a transaction? What's the definition of ACID?

## Frontend

- What is responsive design and how is it achieved?
- What is a CSS preprocessor?
- What is a media query in CSS?
- What’s a CDN?
- How can it help to improve a frontend?
- What kind of CDN have you used?
- What’s caching and how does it work?
- What kind of caches have you used?
- How can you test frontend?
- Have you got any experience with Selenium, Cypress, or Storybook.js?

## React

- What are the benefits of using a virtual DOM in React?
- What is the difference between state and props in React?
- What’s the difference between a class component and a functional component?
- How routing works in React?
- What is the difference between controlled and uncontrolled components in React?
- What is Redux?

## Angular

- What is the difference between ngOnChanges and ngOnInit in Angular?
- What is Angular's change detection mechanism?
- What is an Angular service?
- What is dependency injection in Angular?
- What is Angular routing?
- What is the difference between a component and a directive in Angular?

## Frontend Engineering Scenarios

- What are microfrontends?
- What are the benefits of using micro frontends?
- What is a Progressive Web App (PWA)?
- What are the benefits of using PWA?
- What are the key features of a PWA?
- How can you optimize a PWA for performance?
- Client Side Rendering (CSR) vs Server Side Rendering (SSR), explain the concepts
- Can you describe your approach to optimizing the performance and user experience of a large e-commerce website?
- How would you approach building a highly interactive and responsive web application with real-time updates? E.g. Financial App Stock Market data

# Behavioral (I don't usually ask these questions)

- Describe a time when you disagreed with a team member. How did you resolve the problem?
- Describe a time when you faced a block at work and how you solved it.
- Tell me about a time when you disagreed with a supervisor.
- What is the most difficult/ challenging situation you’ve ever had to resolve in the workplace? 
- Describe a time when you were able to motivate unmotivated team members.
- Tell me about a decision that you’ve regretted and how you overcame it.
- Tell me about a time when you tried something risky and failed.
- Tell me about a time when you were consulted for a problem.
- Explain a time when you took the initiative on a project.
- What’s the best idea you’ve come up with on a team-based project?
- Tell me about a time when you worked well under pressure.
- So, tell me a bit about yourself…
- Why do you want to work here?
- Where do you see yourself in X years? (X = 3, 5, 10)
- What do you do outside of work?
- What are your strengths and weaknesses?
- Why are you leaving your current job? (not for interns/new grad)
- Who is your idol?
- What is your favorite book?
- Why startup|big tech|[insert here kind of company or industry]?
- How do you see [insert here industry] in the next 5 years?

# Outro
- Are you happy with our salary offering?
- What benefit would you like to see listed?
- What benefit are you glad we offer?
- What is your notice period?
- When would you be available to start?
- Do you have any questions for me?
