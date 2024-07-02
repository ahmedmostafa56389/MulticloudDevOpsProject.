# Ivolve Final project
__-__-__-__-__-__

# MultiCloudDevOpsProject
This final project is about how to deploy an application to openshift cluster using deffirint tools
In this project i use many tools such as: - Docker for contranitaziton and use some another tools as a container 
                                          - Ansible used for run ansible roles and manage configuration " used it in two deffirint ways "
                                          - Jenkins used for CI/CD "use it as a container or installed on localhost "
                                          - Terraform used for Infrastructure provisioning
                                          - OpenShift to deploy the application
                                          - SonaQube for code Quality test

## Project Diagram

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/9b478343-8a6c-4c39-8eb1-d5c90dd8db17.svg" >

## Project Structure
```bash
├── ansible
│   ├── ansible.cfg
│   ├── docker
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── inventory
│   ├── ivolve.pem
│   ├── jen-conf
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   ├── configure_jenkins.yml
│   │   │   ├── install_plugins.yml
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── jenkins
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── jenkins_user
│   │   ├── 2q
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── oc
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── playbook.yml
│   ├── sonar
│   │   ├── compose
│   │   │   └── compose.yaml
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   └── sonarqupe
│       ├── defaults
│       │   └── main.yml
│       ├── files
│       ├── handlers
│       │   └── main.yml
│       ├── meta
│       │   └── main.yml
│       ├── README.md
│       ├── tasks
│       │   └── main.yml
│       ├── templates
│       ├── tests
│       │   ├── inventory
│       │   └── test.yml
│       └── vars
│           └── main.yml
├── ansible2
│   ├── ansible.cfg
│   ├── docker
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── git
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── inventory
│   ├── ivolve.pem
│   ├── jenkins
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── openshift
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── files
│   │   ├── handlers
│   │   │   └── main.yml
│   │   ├── meta
│   │   │   └── main.yml
│   │   ├── README.md
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   ├── tests
│   │   │   ├── inventory
│   │   │   └── test.yml
│   │   └── vars
│   │       └── main.yml
│   ├── playbook.yml
│   └── sonarqube
│       ├── defaults
│       │   └── main.yml
│       ├── files
│       ├── handlers
│       │   └── main.yml
│       ├── meta
│       │   └── main.yml
│       ├── README.md
│       ├── tasks
│       │   └── main.yml
│       ├── templates
│       ├── tests
│       │   ├── inventory
│       │   └── test.yml
│       └── vars
│           └── main.yml
├── build.gradle
├── Dockerfile
├── gradle
│   └── wrapper
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradlew
├── gradlew.bat
├── jenkinsfile
├── openshift
│   ├── deploy.yml
│   ├── route.yml
│   └── service.yml
├── README.md
├── settings.gradle
├── src
│   └── main
│       ├── java
│       │   └── com
│       │       └── example
│       │           └── demo
│       │               ├── controller
│       │               │   └── HomeController.java
│       │               └── DemoApplication.java
│       └── resources
│           ├── application.properties
│           └── templates
│               └── index.html
└── terraform
    ├── main.tf
    ├── modules
    │   ├── cloudwatch-sns
    │   │   ├── main.tf
    │   │   └── variables.tf
    │   ├── ec2
    │   │   ├── main.tf
    │   │   ├── outputs.tf
    │   │   └── variables.tf
    │   ├── security-groups
    │   │   ├── main.tf
    │   │   ├── outputs.tf
    │   │   └── variables.tf
    │   └── vpc
    │       ├── main.tf
    │       ├── outputs.tf
    │       └── variables.tf
    ├── output.tf
    ├── terraform.tfstate
    ├── terraform.tfstate.backup
    ├── terraform.tfvars
    └── variables.tf
```

# First stage 

## Terraform

Terraform is a powerful tool used for infrastructure provisioning and management. It allows developers and operators to define infrastructure as code (IaC), using a declarative configuration language. With Terraform, you can describe the components of your cloud infrastructure (like servers, databases, and networking) in configuration files. Terraform then automatically manages the lifecycle of these resources, provisioning and configuring them as needed to match the desired state defined in your code. This approach improves reproducibility, consistency, and efficiency in managing infrastructure across different cloud providers and environments.

- **Step 1: Terraform Initialization**:
  - Initializes Terraform to set up the environment and modules required for deployment.
  - Ensures Terraform plugins are installed and initializes backend configurations.

   ![Alt text](screenshots/terraform-init.png)

- **Step 2: Terraform plan**:
"The `terraform plan` command in Terraform generates and displays an execution plan. It analyzes the current state of infrastructure defined in your Terraform configuration files (`*.tf`) and compares it with the desired state. The output outlines the actions Terraform will perform: creating, modifying, or deleting resources, along with any associated attributes changes. Importantly, `terraform plan` only previews these changes without applying them, allowing users to review and validate proposed modifications before execution."

- **Step 3: Terraform Apply**:
 - used to apply all changes in terraform configuration files 

    ![Alt text](screenshots/terraform-1.png)
    
    ##########################################

    ![Alt text](screenshots/terraform-2.png)


- **Stage 5: Terraform output**:

Terraform output files define values that are displayed post-deployment, like IP addresses or URLs. They're defined in `outputs.tf`, using `output` blocks with unique names and expressions. Accessed via `terraform output`, they facilitate integration and automation by sharing deployment details across infrastructures.


  - Usea terraform output cinfiguration file to get the ip of AWS EC2 to use it in ansible inventory for applying ansible tasks
    and also get another information such as : - subnets IPs
                                               - VPC ID

__-__ __-__ __-__ __-__ __-__ __-__ __-__ __-__

# Socend stage 
## Ansible

Ansible is an open-source automation tool used for configuration management, application deployment, and task automation. It simplifies IT operations by allowing users to automate repetitive tasks through declarative YAML-based playbooks. Ansible uses SSH to communicate with remote nodes and does not require any agents to be installed on them, making it lightweight and easy to set up. Its modular design and extensive community support make it a popular choice for managing infrastructure as code and orchestrating complex IT workflows efficiently.

**Resources: https://docs.ansible.com/**

**in this stage i take to ways**

### First way "continarization"

Containers, particularly through technologies like Docker, revolutionize software development and deployment by encapsulating applications and their dependencies into lightweight, portable units. These containers include everything needed to run an application: code, runtime, system tools, libraries, and settings. Here's a brief overview of how containers, such as Docker containers, manage and limit resources on a localhost:

1. **Resource Isolation**: Containers utilize Linux kernel features like namespaces and cgroups to provide isolated environments for applications. Each container operates as if it has its own dedicated resources, such as network interfaces, file systems, and process trees. This isolation prevents applications from interfering with each other and provides a level of security by limiting what each container can access.

2. **Resource Allocation**: Docker containers allow developers to specify resource limits for each container instance. These limits can include CPU shares, memory usage, disk I/O, and network bandwidth. By setting these constraints, developers can ensure that no single container monopolizes resources, leading to a more stable and predictable environment.

3. **Efficient Resource Utilization**: Containers optimize resource usage by sharing the host operating system's kernel. Unlike virtual machines (VMs), which require their own operating system instance, containers leverage the host OS's kernel, making them lightweight and efficient. This efficiency means more containers can run on the same host without significant performance degradation, thus maximizing resource utilization.

4. **Portability and Consistency**: Containers ensure consistency across different environments, from development to production. Since each container encapsulates its dependencies and configuration, applications behave consistently regardless of where they run. This portability simplifies deployment workflows and reduces the likelihood of issues arising from differences between development and production environments.

In summary, containers like Docker provide a standardized, efficient way to package, deploy, and manage applications while limiting resource usage on a localhost through isolation and resource allocation mechanisms. This approach not only enhances scalability and efficiency but also improves developer productivity by streamlining the deployment process.

### Steps

in this way we fucas to use ansible roles,

**what is ansible roles**

Ansible roles are modular units that organize tasks, configurations, and files into reusable packages. They enhance playbook organization, promote code reuse across projects, and simplify managing complex automation tasks by encapsulating functionality in a structured directory format. Roles enable efficient collaboration, inheritance of configurations, and consistent automation across environments, contributing to scalable and maintainable Ansible deployments.

##### 1- intialize ansible roles 

**to install Docker and all it's dependencies**
Tasks:
```
vim ~/project/ansible2/docker/tasks/main.yml
```
1. Update apt packages
2. Gither destribuation information
3. Install all  Docker Prerequsites 
4. Add Docker GPG Key
5. Add Docker repository
6. Install Docker
7. Start and Enable Docker service
8. Change the permation for /var/run/docker.sock

#####################################################

**to install jenkins and all it's dependencies**
Tsaks:
```
vim ~/project/ansible2/jenkins/tasks/main.yml
```
1. Pull jenkins image
2. Create jenkins container
3. Fetch jenkins Password
4. Install Java 17 for jenkins conatainer
5. Install Docker Cli inside jenkins conatiner

########################################################

**to install git inside jenkins conatiner**
Tasks:
```
vim ~/project/ansible2/git/tasks/main.yml
```
1. Update apt Cash
2. Install Git
##########################################################
**to install OpenShift inside jenkins conatiner**
Tasks:
```
vim ~/project/ansible2/openshift/tasks/main.yml
```
1. Install oc cli on the localhost
2. Copy oc cli to jenkins container
3. Extract oc cli tallbar inside jenkins container
4. Ensure that oc cli is executable inside jenkins container

###########################################################

**to itiate sonarqube server**
- What is sonarQube ?

SonarQube is an open-source platform designed to continuously inspect code quality throughout the software development lifecycle. It provides a comprehensive range of static code analysis tools to identify bugs, security vulnerabilities, code smells, and enforce coding standards across multiple programming languages.

Key features of SonarQube include:

1. **Static Code Analysis**: It scans codebases to detect issues early in the development process, helping teams maintain clean, reliable code.

2. **Code Quality Metrics**: SonarQube calculates various metrics such as code coverage, complexity, duplications, and maintainability to assess overall code health.

3. **Security Vulnerability Detection**: It identifies potential security vulnerabilities in code, such as SQL injection, XSS, and other common vulnerabilities.

4. **Integration with CI/CD**: SonarQube integrates seamlessly with Continuous Integration (CI) and Continuous Deployment (CD) pipelines, enabling automated code analysis and quality checks as part of the build process.

5. **Customizable Rules and Profiles**: Teams can tailor SonarQube's analysis rules and quality profiles to fit specific project requirements and coding standards.

6. **Historical Reporting and Trends**: It provides historical data and trend analysis, allowing teams to track improvements in code quality over time and prioritize technical debt reduction.

Overall, SonarQube is widely used in software development teams to ensure code reliability, security, and maintainability by catching issues early and fostering continuous improvement in code quality.


**Resources: https://docs.sonarsource.com/sonarqube/latest/**

Tasks:
```
vim ~/project/ansible2/sonaqube/tasks/main.yml
```
1. Create Docker volumes for sonarqube
2. Pull PostgreSQL image
3. Run PostgreSQL container
4. Pull SonarQube image
5. Run SonarQube container

##############################################

##### 2- get the SSH Key that attached to EC2
- get the SSH Key for EC2 to enable ansible to connect to EC2 Via SSH

  ![Alt text](screenshots/SSH-terraform.png)
  ![Alt text](screenshots/SSH-ansible.png)

- and note to call the SSH key path on "ansible.cfg" file 

![alt text](<Screenshot (98).png>)

##### 3- Run ansible playbook


```sh
ansible-playbook -i inventory playbook
```
![alt text](ansible(2)-3.png)


__-__ __-__ __-__ __-__ __-__ __-__ __-__ __-__ __-__

### Second way "Install on local machine"

In This way I install every thing on the local machine "but it need more resources"

I will install the same package " 'Docker' , 'Jenkins' , 'git' , 'openshify' "

create SonarQube as a docker compose 

  ![Alt text](screenshots/ansible-1.png)

###############################################
### steps

##### 1- Intiate ansible roles
**install docker and its pre-requistes**
Tasks:
```
vim ~/project/ansible/docker/tasks/main.yml
```
The Same tasks for the first way

##############################################

**install jenkins on localhost**
Tasks:
```
vim ~/project/ansible/jenkins/tasks/main.yml
```
1. Install Java 
2. install openJDK 17
3. Download jenkins repository key
4. Add jenkins to repository
5. Install jenkins 
6. start jenkins service

#############################################

**Configure jenkins and create user**
Tasks:
```
vim ~/project/ansible/jenkins_user/tasks/main.yml
```
1. Add jenkins Password
2. Create CRUMB authentication request
3. Add jenkins administration account
4. Install jenkins plugns
5. DAEMON reload 
6. restart jenkins service

############################################

**install OpenShift CLI**
Tasks:
```
vim ~/project/ansible/oc/tasks/main.yml
```
1. Install oc cli
2. Extract OpenShift CLI
3. verify installation

###########################################

**install and configure SonarQube**
Tasks:
```
vim ~/project/ansible/sonarqube/tasks/main.yml
```
Create Docker compuse to run sonarqube
1. Copy docker compuse to the managed host 
2. Set sysctl and ulimit settings for ElasticSearch
3. Ensure compose.yml file exists
4. Change permissions of compose.yml file 
5. Run Docker Compose
```sh
docker compose -f /home/ubuntu/compose.yaml up -d
```
###########################################

##### 2- get the SSH Key that attached to EC2
- get the SSH Key for EC2 to enable ansible to connect to EC2 Via SSH

###########################################

##### 3- Run Ansible playbook

![alt text](ansible(1)-1.png)
![alt text](ansible(1)-2.png)
![alt text](ansible(1)-3.png)
![alt text](ansible(1)-4.png)
![alt text](ansible(1)-5.png) 

__-__ __-__ __-__ __-__ __-__ __-__ __-__ __-__ __-__

# Third Stage
## OpenShift

**What is OpenShift Cluster**

An OpenShift cluster is a scalable, container-centric platform built on Kubernetes that enables organizations to deploy, manage, and orchestrate containerized applications. It consists of a collection of nodes (servers) that work together to provide a unified platform for running applications. 

Key components of an OpenShift cluster include:

1. **Master Nodes:** Control plane components that manage and coordinate the cluster. They include API server, scheduler, controller manager, and etcd (a distributed key-value store for cluster data).

2. **Worker Nodes:** Also known as compute nodes, these run the containerized applications using Kubernetes pods. They host the application containers and necessary services like networking and storage.

3. **Networking:** OpenShift uses software-defined networking to enable communication between pods and services within the cluster and with external networks.

4. **Storage:** Provides persistent storage solutions for applications, allowing data to persist beyond the lifespan of individual containers.

5. **Operators:** Automation controllers that extend Kubernetes to manage complex, stateful applications on behalf of the user, ensuring easier management of applications running in the cluster.

6. **Console and CLI:** Provides graphical and command-line interfaces for developers and administrators to interact with and manage the cluster, monitor resources, deploy applications, and configure services.

OpenShift clusters support high availability configurations, allowing for redundancy and fault tolerance across nodes and components. They are designed to simplify the deployment and management of containerized applications at scale, offering features for application lifecycle management, security, and integration with CI/CD pipelines.


**Resources: https://docs.openshift.com/**

_____________________________________________________
_____________________________________________________

we need to create a Deployment file to apply create a deployment with four replacis 

![Alt text](screenshots/deploy-yaml.png)

And Then Expose this deployment and get the service  with port 8080

![Alt text](screenshots/service-yaml.png)




##### 2- Clone the App using this command
```bash
git clone https://github.com/EngMohamedElEmam/spring-boot-app.git
```

##### 3- push to your new repo 
```bash
git add .
git commit -m "push the app"
git push https://github.com/saeedkouta/MultiCloudDevOpsProject.git
```

##### 4- Create A new Branch called "dev"
```bash
  git checkout -b dev
```
dev Branch: Used for development work.

### Step 2: Infrastructure Provisioning with Terraform

##### What is Terraform?

Terraform is an open-source Infrastructure as Code (IaC) tool created by HashiCorp. It allows users to define and provision data center infrastructure using a high-level configuration language. By writing declarative configuration files, users can specify the desired state of their infrastructure, and Terraform will handle the creation, update, and deletion of resources to match that state.

##### Purpose of Terraform

The primary purpose of Terraform is to enable consistent, reproducible, and automated infrastructure management. It helps to:

1. **Simplify Infrastructure Management**: By using configuration files, Terraform makes it easy to manage and version control infrastructure changes.
2. **Ensure Consistency**: Terraform provides a unified way to define infrastructure, ensuring consistency across environments and reducing configuration drift.
3. **Improve Collaboration**: Teams can collaborate on infrastructure changes by reviewing and version controlling Terraform configuration files.
4. **Enable Infrastructure as Code (IaC)**: Terraform allows infrastructure to be treated as code, which means it can be tested, validated, and automated like software code.
5. **Multi-Cloud and Provider Agnostic**: Terraform supports multiple cloud providers and services, allowing for a consistent approach to infrastructure management across different environments.

Using Terraform, organizations can achieve greater efficiency, reliability, and scalability in their infrastructure operations, leading to faster deployment cycles and reduced operational overhead.

##### Overview
[**Terraform Modules README file**](https://github.com/saeedkouta/MultiCloudDevOpsProject/tree/dev/terraform#readme)

This README file documents my process of creating Terraform modules. It includes all the necessary steps in details and screenshots of the configurations used in each module.

### Step 3: Configuration Management with Ansible

#### What is Ansible?

Ansible is an open-source automation tool that simplifies the configuration management, application deployment, orchestration, and task automation across multiple systems. Developed by Red Hat, Ansible uses a declarative language to describe system configurations, known as playbooks, which are written in YAML format. These playbooks define the desired state of systems and automate the deployment and management tasks needed to achieve that state.

#### Purpose of Ansible

The primary purpose of Ansible is to automate IT tasks that are repetitive, complex, or time-consuming. It serves several key purposes:

1. **Configuration Management**: Ansible allows you to define and enforce the desired state of your infrastructure, ensuring consistency and reducing configuration drift.
2. **Application Deployment**: Ansible facilitates the deployment of applications by automating the necessary steps and configurations across multiple servers or environments.
3. **Orchestration**: Ansible can orchestrate complex workflows involving multiple systems, such as rolling updates, system provisioning, and cloud management.
4. **Task Automation**: It automates routine tasks, freeing up administrators' time for more strategic activities.
5. **Agentless Architecture**: Ansible operates over SSH or PowerShell, making it lightweight and easy to deploy without needing agents installed on managed systems.
6. **Integration and Extensibility**: Ansible integrates with existing tools and technologies and can be extended through modules and plugins to support a wide range of use cases.

By leveraging Ansible, organizations can achieve greater operational efficiency, improve scalability, ensure compliance, and accelerate time-to-value for their IT infrastructure and applications.

#### Overview
[**Ansible Roles README file**](https://github.com/saeedkouta/MultiCloudDevOpsProject/blob/dev/ansible-roles/README.md)

This README file details the creation and use of Ansible Roles for automation tasks. It includes comprehensive steps, configuration details, and screenshots illustrating the setup and execution of each role.

### Step 4: Configure Jenkins to Run the Pipeline

#### what is Jenkins ?

Jenkins is an open-source automation server widely used for continuous integration and continuous delivery (CI/CD). It allows developers to automate the building, testing, and deployment of applications, facilitating faster and more reliable software development. Jenkins supports a vast array of plugins to integrate with various development, testing, and deployment tools, making it highly flexible and customizable to suit different project needs. Its primary purpose is to streamline the software development lifecycle, ensuring code changes are continuously integrated and delivered efficiently.

#### 1- Open Jenkins and Add the Required Credintials 

#### To Add Credintials go to `manage jenkins` > `Credintials`

#### 1.1 GitHub Credentials

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/a7f7321e-c5b8-4ef8-af36-0534a55f8fcc" width="1000" >

#### 1.2. AWS Access Key:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/8f4357dc-a5ed-4bb7-a04d-00d765c7f3aa" width="1000" >

#### 1.3. AWS Secret Access Key:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/a7493c72-a904-4165-801c-4fd2a5c972b7" width="1000" >

#### 1.4. The SSH Key Pair:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/e951deee-1854-4d55-8f5a-3c3bd68e6734" width="1000" >

### Step 5: Create and Build The pipeline

#### 1- Create A new Pipeline:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/535652d7-e17b-4503-b374-a6d01e3406a9" width="1000" >

#### 2- Add the repo and the github credintials and choose the branch:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/c85fe234-daf5-4db7-97c1-8b50f09f0443" width="1000" >

#### 3- Add the name of the jenkinsfile:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/e94f3cae-5bdc-4f52-bdbb-47f348e0c67f" width="1000" >

#### 4- Build the pipeline:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/62dd7c12-5372-431a-917f-e3c3d6463167" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/68691174-48c6-4465-b88f-329d7f614fcb" width="1000" >

### Step 6: Show the provisioned infrastructure

 it's in the last part of [**Terraform Modules README file**](https://github.com/saeedkouta/MultiCloudDevOpsProject/tree/dev/terraform#readme)

### Step 7: Test The Monotoring 

#### 1- Check the Cloud Watch Alarms 
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/b20a7c57-4658-43b2-9cb2-d58d200e2874" width="1000" >

#### 2- Check sns topic and confirm the subscreption
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/03acf5ac-2cce-475d-8f7c-2e72651d1a8b" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/80917f0f-9583-419b-8637-9bc58b58b87c" width="1000" >

#### 3- Create script to load the cpu:
[**Load-script.sh**](https://github.com/saeedkouta/MultiCloudDevOpsProject/blob/dev/scripts/load-script.sh)

#### Run it Twice ivolve.sh & script.sh :
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/64887c3a-34da-42f5-849c-775453f0b5ef" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/0a88feab-37d1-46c7-9881-26c0dc2a9602" width="1000" >

#### 4- check the Cloud Watch Alarms Again :
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/041282cc-1d37-4c63-866b-10fb41b8887c" width="1000" >

#### the cpu utilization comes above 60% For more than 5 minutes
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/d86eaa32-4960-4f3c-bb6e-7e28527d8df8" width="1000" >

#### 5- Check the Gmail For the Sns Email:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/d59154d5-81f4-4dd2-8a9c-7281af07eec6" width="1000" >

## Pipeline 2: Jenkins, SonarQube, Docker, OpenShift Integration

The second Jenkins pipeline integrates SonarQube with Jenkins using a shared library and orchestrates application deployment to an OpenShift cluster:

- **Stage 1: Git Checkout**:
  - Checks out the application source code repository from Git.

- **Stage 2: Unit Test**:
  - Executes unit tests on the checked-out codebase to ensure code quality and functionality.

- **Stage 3: SonarQube Analysis**:
  - Performs static code analysis using SonarQube to detect bugs, vulnerabilities, and code smells.
  - Provides detailed reports and metrics for code quality improvement.

- **Stage 4: Build and Push Docker Image**:
  - Builds the Docker image for the application based on the codebase.
  - Pushes the built Docker image to DockerHub or another container registry for versioning and distribution.

- **Stage 5: Deploy to OpenShift**:
  - Deploys the application as a containerized service on an OpenShift cluster.
  - Creates necessary Kubernetes resources (deployment, service) and exposes the service for external access.

### Integration with [Shared Library](https://github.com/saeedkouta/MultiCloudProject_shared_library.git)

pipelines utilize a shared library in Jenkins to encapsulate and reuse pipeline logic across different projects, promoting consistency and efficiency in pipeline management.

### Benefits of Automation

- **Efficiency**: Automates infrastructure provisioning and software deployment, reducing manual effort and potential errors.

- **Quality Assurance**: Integrates automated testing and code analysis to maintain high code quality standards throughout the development lifecycle.

- **DevOps Practices**: Implements DevOps principles by automating CI/CD processes and promoting collaboration between development and operations teams.
 
### Step 1: Openshift Deployment and Service files

#### What is OpenShift?
OpenShift is a Kubernetes-based platform that provides a robust and scalable environment for container orchestration and application deployment. Its purpose is to streamline the development, deployment, and management of containerized applications by offering a comprehensive suite of developer and operational tools, integrated CI/CD pipelines, automated scaling, and application monitoring capabilities. OpenShift aims to enhance productivity, ensure application reliability, and foster rapid innovation by providing a consistent and secure infrastructure across hybrid and multi-cloud environments
 
#### Overview
[**Openshift README file**](https://github.com/saeedkouta/MultiCloudDevOpsProject/blob/dev/ansible-roles/README.md)

This README file details the creation and use of openshift deployment. It includes comprehensive steps, configuration details, and screenshots of openshift deployment and service.

### Step 2: Create openshift ServiceAccount and give it role then Extract the token
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/84c45259-c4a8-47a0-ac33-ffdc0154b75f" width="1000" >

### Step 3: Access to the SonarQube Container

#### SonarQube Overview

**SonarQube** is an open-source platform used for continuous inspection of code quality. It performs automatic reviews with static analysis of code to detect bugs, code smells, and security vulnerabilities. SonarQube supports various programming languages and integrates seamlessly with CI/CD pipelines.

#### Purpose:

- **Improving Code Quality**: SonarQube analyzes code to identify potential issues, ensuring high-quality, maintainable code.
- **Security**: It helps in detecting security vulnerabilities early in the development process.
- **Technical Debt Management**: SonarQube measures technical debt, helping teams understand the effort required to fix code issues.
- **Continuous Integration**: Integrates with CI/CD tools to provide real-time feedback on code quality during the development process.

#### 1- When Accessing sonarqube for the first time its username and password is admin and sonarqube will ask u to change the password before using it
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/c3ba88b5-4386-4d3a-b83f-28e4f6a3c6e7" width="1000" >

#### 2- Create Project :
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/cd76975e-4a42-4d70-a8fa-b047a5e11d39" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/33b89b96-7d06-45da-b5b0-2ca892f546da" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/9699fcf5-3162-499b-a0fb-2129f4a56e97" width="1000" >

#### 3- Get Token:
`administrator` > `security` > `users` > `token`
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/6a5dd509-2e0e-459d-93fa-7c535804724d" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/5b0d3258-df28-4670-8ee7-0f6bdb645c7e" width="1000" >

### Step 3: Access To the jenkins Container and configure it
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/48ff2d68-d43f-46c0-9af7-0dcd68a83d36" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/75b87f6a-8978-4d1f-a7fe-cdafd28183b4" width="1000" >

#### 1- Add Required Credintials:

#### GitHub:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/3d3144b5-9a4d-4773-8f0c-7bff4ba86730" width="1000" >

#### DockerHub:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/8e4a268b-0f81-4a79-9314-6c5caf391913" width="1000" >

#### sonar-token
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/69de2957-dd32-4011-8ac8-abde3c3e36c1" width="1000" >

#### openshift-token
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/a07dc631-2a7b-4675-88ed-9cedd505133c" width="1000" >

#### 2- install sonar-scanner Plugin:
`manage jenkins` > `plugins` > `available plugins`

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/9ac9e5db-e9e5-41f7-81b3-e1c25ab70987" width="1000" >

#### 3- Configure the sonar-scanner tool:
`manage jenkins` > `tools` > `sonarqube-scanner installations`

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/f084794f-1be4-4c91-af7d-c7f787ab358e" width="1000" >

#### 4- Configure SonarQube-server
`manage jenkins` > `system` > `SonarQube Servers`

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/c06fc0d2-8b3b-43e6-b940-be5c120a7adc" width="1000" >

#### 5- Add [Shared_library](https://github.com/saeedkouta/MultiCloudProject_shared_library.git)
`manage jenkins` > `system` > `Global Pipeline Libraries`

<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/59429cc8-5099-4a1d-b0bf-59880208ed52" width="1000" >

### Step 4: Create and Build a Pipeline

#### 1- Create New pipeline
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/91784362-723b-4bb7-8533-234a06601757" width="1000" >

#### 2- Configure the Pipeline:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/85dfd03f-5b26-4cff-8427-e9d162362527" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/a549466e-065e-460a-9074-9de5583d6ffd" width="1000" >

#### 3- Build The Pipeline:

#### Git Checkout Stage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/0a188c50-a081-4d0a-bd45-1ce46899b474" width="1000" >

#### Uint Test Stage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/4b03da5e-0b63-4dd7-9322-1f9d78de9083" width="1000" >

#### SonarQube Analysis Stage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/216b16de-cff0-4ec7-941e-22465c42e8d0" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/bbf35244-79dc-458e-a862-6459ae4ee75a" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/902f75d6-9296-4c9f-b5ed-cb55aa5e0529" width="1000" >

### Build and Push Stage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/6118286f-8135-4754-adb9-b5891ea795e6" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/14d7f56d-044d-4b60-91e8-fc27945d748d" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/7bcbdb3c-a2ab-4929-aa82-d9fac8ee1ccd" width="1000" >

### Deploy To Openshift Stage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/2e7ea5eb-72e0-4f3a-89aa-66e464659272" width="1000" >
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/79486577-0007-4f28-b305-6fa696ffa290" width="1000" >

### the Screenshots of OpenShift components that Created is in the [openshift README file](https://github.com/saeedkouta/MultiCloudDevOpsProject/blob/dev/openshift/README.md) 

### The Application WebPage:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/901f53fb-f0a7-437f-80a8-29d630039f2e" width="1000" >

### Step 5: Create Pull Request

#### 1- Create Pull Request to add the changes to the main branch:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/0f74baf5-0131-4eb2-9883-04fc88acbf7e" width="1000" >

#### 2- Merge pull request:
<img src="https://github.com/saeedkouta/MultiCloudDevOpsProject/assets/167209058/ec942d90-309f-458a-8f62-29977fd5e56d" width="1000" >

## Troubleshooting

### With `Terraform`

#### 1- make sure to increase the ec2 storage. make it at least 20 GB

#### 2- create s3 bucket and dynamoDB table Before run backend module

### With `Ansible-Roles`

#### 1- public key error . i solve it by giving the key a secure permisions **chmod 400 key.pem**

#### 2- ModuleNotFoundError: No module named 'ansible.module_utils.six.moves'

#### it's an error displayed when running the ansible roles using jenkins . i solved it by using python 3.10.12 version with ansible core 2.17

### With `Jenkins`

#### 1- before using jenkins u have to install java 11 or java 17 to be able to work

### With `SonarQube`

#### 1-  first create postgresql database then link it to sonarqube to be able to work

## Documentation Resources

This table provides links to helpful documentation for the used tools and technologies:

| Documentation | Resource Link |
|---|---|
| Ansible | [Ansible Documentation](https://docs.ansible.com/) |
| Ansible Galaxy | [Ansible Galaxy](https://galaxy.ansible.com/) |
| Jenkins | [Jenkins Documentation](https://jenkins.io/doc/) |
| Docker | [Docker Documentation](https://docs.docker.com/) |
| Terraform | [Terraform Documentation](https://www.terraform.io/docs/) |
| OpenShift | [OpenShift Documentation](https://docs.openshift.com/) |
| SonarQube | [SonarQube Documentation](https://docs.sonarqube.org/) |
| PostgreSQL | [PostgreSQL Documentation](https://www.postgresql.org/docs/) |
| Spring Boot | [Spring Boot Documentation](https://spring.io/guides/spring-boot/) |
| GitHub | [GitHub Documentation](https://docs.github.com/) |
| AWS | [AWS Documentation](https://aws.amazon.com/documentation/) |