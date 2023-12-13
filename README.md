# One-week sprint project for a Junior Cloud DevOps Engineer

In this one-week sprint project, our goal is to set up a basic API on Amazon Web Services (AWS) using Terraform for infrastructure provisioning and GitLab CI/CD for automated deployment. As a Junior Cloud DevOps Engineer, we’ll gain hands-on experience with essential tools and practices in the DevOps domain.

## Steps taken building this project
- [x] [Project](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/blob/main/README.md#project-deploying-a-simple-api-on-aws-using-terraform-with-gitlab-cicd)
- [x] [Tips for a Junior DevOps Engineer](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/tree/main#tips-for-a-junior-devops-engineer)
- [x] [Understanding the project requirements and scope](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/tree/main#understanding-the-project-requirements-and-scope)
- [x] [High-Level Architecture](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/blob/main/README.md#high-level-architecture)
- [ ] Draw the High-Level Architecture using Lucidchart or Draw.io
- [x] Set up an AWS account
- [x] Set Up Billing Alarms and Budgets
- Create billing alarms to receive notifications when costs exceed predefined thresholds. This helps prevent unexpected expenses.
- Set up budgets to monitor and control spending. It allows you to set spending limits and receive alerts when nearing or surpassing the defined budget.
- [x] Configure AWS Identity and Access Management (IAM)
- Create IAM Users
- Define IAM Groups
- Assign Permissions
- Secure Access Keys
- Set User Password using the console
- Sign in using the created IAM User
- [x] Configure necessary permissions on AWS account
- [x] Install Terraform
- [ ] Set up GitLab CI/CD


### Project: Deploying a Simple API on AWS Using Terraform with GitLab CI/CD

Working on a mini project within a week can be a great way to dive into cloud DevOps! Here's a plan for a one-week sprint involving AWS, Terraform, and GitLab CI/CD:

| **Day**     | **Tasks**                                                                                      |
|-------------|------------------------------------------------------------------------------------------------|
| **Day 1**   | **Planning and Setup**                                                                         |
|             | - Understand the project requirements and scope                                                |
|             | - Set up an AWS account and configure necessary permissions                                    |
|             | - Draw the High-Level Architecture using Lucidchart or Draw.io                                 |
|             | - Install Terraform and GitLab CI/CD tools                                                      |
|             | - Initialize a new GitLab repository for the project                                            |
| **Day 2**   | **Infrastructure Setup with Terraform**                                                        |
|             | - Define infrastructure requirements (e.g., VPC, Subnets, Security Groups) using Terraform     |
|             | - Create Terraform files for EC2 instance(s) or another service for your API deployment         |
| **Day 3**   | **AWS Configuration and Deployment**                                                            |
|             | - Apply Terraform configuration to create infrastructure on AWS                                 |
|             | - Configure AWS services (like EC2 or any other service) for hosting your API                   |
|             | - Test manually to ensure the deployed infrastructure is functional                             |
| **Day 4**   | **Code API and Set Up GitLab CI/CD Pipeline**                                                  |
|             | - Develop a simple API using a language/framework of your choice                                 |
|             | - Create necessary scripts (build, test, deploy) for the CI/CD pipeline                         |
|             | - Configure `.gitlab-ci.yml` for automated testing and deployment                                |
| **Day 5**   | **CI/CD Testing and Refinement**                                                                |
|             | - Push code changes to GitLab and observe the CI/CD pipeline in action                           |
|             | - Debug and refine the pipeline as needed (handling errors, improving tests)                     |
| **Day 6**   | **Documentation and Finalization**                                                              |
|             | - Document the project: Infrastructure setup, CI/CD workflow, and any troubleshooting steps       |
|             | - Review the project to ensure completeness and functionality                                   |
|             | - Prepare a demo or presentation to showcase your project                                        |
| **Day 7**   | **Presentation and Wrap Up**                                                                   |
|             | - Practice your demo/presentation                                                                |
|             | - Present your project to colleagues, mentors, or peers                                          |
|             | - Reflect on your learnings and note areas for improvement                                       |

#### Tips for a Junior DevOps Engineer:

- **Start Simple:** Begin with a basic project setup and gradually add complexity. Don't try to incorporate advanced features at the beginning.
- **Documentation Is Key:** Keep detailed notes throughout the project. This will help you understand your own process and make troubleshooting easier.
- **Use Online Resources:** Leverage AWS and Terraform documentation, tutorials, and forums. Don't hesitate to seek help from communities if you're stuck.
- **Regular Commits:** Commit your changes frequently and write meaningful commit messages. This helps in tracking changes and debugging.
- **Test Thoroughly:** Ensure your CI/CD pipeline includes proper testing phases. This practice enhances the reliability of your deployments.

Remember, this plan is flexible and might need adjustments based on your progress and familiarity with the tools. Good luck with your project!

## Understanding the project requirements and scope

Understanding the project requirements and scope means figuring out exactly **what you need to do** and **what your project will involve**.


**Project Goal (The main aim is to):**
1. create a basic API (a way for different software programs to talk to each other)
2. deploy the basic API on Amazon Web Services (AWS)
3. use Terraform for setting up infrastructure
4. GitLab CI/CD (Continuous Integration/Continuous Deployment - a way to automate testing and deploying code).

**Key Questions to Answer:**
1. What does the API need to do? (e.g., handle certain types of data, perform specific tasks)
   - Use Python to make a GET request to an API using the popular requests library
   - The API needs to handle user authentication
   - Perform CRUD operations.
3. Which AWS services will you use? (e.g., EC2 for hosting, maybe others for databases or storage, Deploying a basic API on AWS can be done using various services, but one common approach is to use AWS Lambda for the code execution and API Gateway to manage the API endpoints)
   - AWS Lambda for code execution, API Gateway for managing API endpoints, and Amazon RDS for database storage.
4. How will you set up the infrastructure using Terraform? (e.g., networks, servers)
  - Set up VPC, subnets, security groups, Lambda function configuration, API Gateway, and IAM roles using Terraform.
5. What steps are required to automate testing and deployment using GitLab CI/CD? (e.g., writing scripts, setting up pipelines)
  - Write test scripts for API endpoints, set up GitLab pipelines for automated testing (unit, integration) and deployment to AWS.

**Scope: Define the boundaries of your project. For example:**
1. Which parts of AWS will you use? (Avoid making it too complex at first)
  - Utilize AWS Lambda and API Gateway
2. What level of complexity will your API have? (Start with a simple one and maybe add features later)
  - Begin with a simple API 
3. What specific tasks will you perform with Terraform and GitLab CI/CD? (Setting up infrastructure, automating testing and deployment)
- Terraform: Network and server setup; GitLab CI/CD: Automation of testing and deployment

**Constraints and Resources: Consider any limitations or resources available to you:**
1. Time: One week to complete this project.
2. Skills: What do you already know? What might you need to learn?
  - Knowledge in Python to build API
  - Learn how to use AWS Lambda and API Gateway
  - Learn how to code AWS infrastracture using Terraform 
3. Tools: Are there any specific versions or tools you're required to use?

| Tool           | Required Version/Specification        | Purpose                                               |
|----------------|--------------------------------------|-------------------------------------------------------|
| AWS    | AWS Account                                  | Hosting the API on AWS                                 |
| Terraform      | >= v0.12.0                            | Setting up infrastructure on AWS                       |
| GitLab CI/CD         | GitLab account, GitLab Runner   | Version control and CI/CD automation                    |
| AWS CLI        | >= v2.0.0                             | Command-line access to AWS services                    |
| Programming Language/Framework for API | Python/Flask | Creating the API                           |
| AWS Lambda          | -                                    | Executing the API code                            |
| AWS API Gateway     | -                                    | Managing API endpoints                            |
| AWS IAM             | -                                    | Managing access to AWS services                   |
| AWS VPC             | -                                    | Creating virtual networks                         |
| AWS EC2 (optional)  | -                                    | Alternative for hosting the API, if not using Lambda |

These tools and services play specific roles in the project:

- **AWS:** Your AWS account will host the API, and services like IAM, VPC, Lambda, API Gateway, and EC2 (if chosen) will be utilized.
- **Terraform:** Used to automate the setup of AWS infrastructure for hosting the API.
- **GitLab CI/CD:** Helps in automating tests and deploying the code.

Please adjust the versions and tools based on your project requirements or any specific guidelines from your team or organization.


## High-Level Architecture:

1. **AWS Services Used:**
   - **AWS Lambda:** Executes the API code.
   - **AWS API Gateway:** Manages API endpoints and directs requests to Lambda.
   - **AWS IAM:** Manages access to AWS services.
   - **AWS VPC:** Creates a virtual network for resources.
   
2. **Terraform Configuration:**
   - **Networking:** Defines VPC, subnets, and security groups.
   - **Lambda & API Gateway:** Configures these services with necessary settings.
   - **IAM Roles:** Sets up roles for Lambda execution and other permissions.

3. **GitLab CI/CD:**
   - **Pipeline Configuration:** Contains stages for testing and deployment.
   - **Testing Steps:** Runs automated tests on the code.
   - **Deployment Steps:** Pushes the code changes to AWS services using Terraform.

4. **Workflow Overview:**
   - Developer pushes code changes to GitLab repository.
   - GitLab CI/CD pipeline triggers.
   - Pipeline runs tests on the code.
   - Upon successful tests, Terraform applies changes to AWS infrastructure.
   - Updated code gets deployed to Lambda via GitLab CI/CD.

### Textual Representation:

```
AWS Architecture:
- VPC
  - Subnets
  - Security Groups

AWS Services:
- Lambda Function
- API Gateway
- IAM Roles

Terraform Configuration:
- Networking Setup (VPC, Subnets)
- Lambda & API Gateway Configuration
- IAM Role Definitions

GitLab CI/CD Pipeline:
- Test Stage
- Deployment Stage
  - Terraform Applies Changes
  - Code Deployment to Lambda
```
