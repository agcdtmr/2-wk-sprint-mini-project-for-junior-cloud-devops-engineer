# Two-week sprint project for a Junior Cloud DevOps Engineer

Over the course of a two-week sprint, our objective is to establish a fundamental Python-based API using Docker containers, employing Terraform for infrastructure provisioning on Amazon Web Services (AWS). Additionally, we'll integrate GitLab CI/CD for automated testing and deployment, offering hands-on experience in crucial DevOps tools and practices.

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
- `arch -x86_64 brew install terraform`
- [x] Initialize a new GitLab repository for the project
- [x] [Connect laptop to GitLab using SSH to use the project repo locally](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/blob/main/README.md#connect-your-laptop-to-gitlab-using-ssh-youll-need-to-follow-these-general-steps)
- [x] Clone the repository to your local machine.
- [x] Set up GitLab CI/CD
- Created a template for a .gitlab-ci-cd.yml file that defines stages, jobs, and their configurations to deploy a simple API, make a GET request using Python's requests library, and includes testing as well as build and deploy stages.
- [x] Setup AWS Credentials:
- Set up AWS credentials on your local machine. You can either use the AWS CLI aws configure command or set environment variables (AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY) with your AWS credentials.
- `aws configure list`
- [x] Choose an API to use https://api.publicapis.org/entries
- [x] Create a requirements.txt file
- create requirements.txt file manually and add the dependencies
- [x] Automate the installation
- `pip install -r requirements.txt`
- [x] Brief guide on [how to use the API](https://github.com/agcdtmr/1-wk-sprint-mini-project-for-junior-cloud-devops-engineer/blob/main/README.md#brief-guide-on-how-to-use-the-api)
- [ ] Plan Docker integration for API containerization.
- [x] Create a Dockerfile to containerize API using Docker, we'll need to create a Dockerfile to specifies how to build the Docker image for the application.
- [ ] Write [Getting Started](https://github.com/agcdtmr/2-wk-sprint-mini-project-for-junior-cloud-devops-engineer/blob/main/README.md#getting-started)
- [x] Identify necessary scripts for Docker image creation.
- Dockerfile: This file contains instructions to build the Docker image. It outlines the steps needed to set up the environment, install dependencies, and configure the container. The example Dockerfile provided earlier is crucial for defining the image's configuration.
- Requirements File (requirements.txt): For Python applications, this file lists all the Python dependencies required for your application to run. It allows Docker to install these dependencies within the container during the image build process. The requirements.txt file example was provided earlier in the Flask API containerization example.
- Application Code: Ensure all the necessary application files, including your Flask application (app.py), are present in the directory where you build the Docker image. These files will be copied into the Docker container using instructions within the Dockerfile.
- [x] Set up GitLab CI/CD pipeline for build, test, and deployment
- Configured stages for build, test, validation, and deployment to development and production environments using Docker, AWS, and Terraform. Included necessary installations, testing procedures, and deployment steps. Outputs development and production URLs after successful deployment.

## Project: Deploying a Simple API on AWS Using Terraform with GitLab CI/CD

### Prerequisites:

- AWS Account: Set up an AWS account if you haven't already.
- GitLab Account: Sign up for a GitLab account.
- Install Terraform: Install Terraform on your local machine.
- Configure AWS CLI: Set up AWS CLI on your local machine to authenticate with AWS.
- Docker: Transform the API into a Docker container for deployment.




| **Day**     | **Tasks**                                                                                      |
|-------------|------------------------------------------------------------------------------------------------|
| **Day 1**   | **Planning and Setup**                                                                         |
|             | - [x] Understand the project requirements and scope                                                |
|             | - [x] Set up an AWS account and configure necessary permissions                                    |
|             | - Visualize High-Level Architecture using diagramming tools. ex. Lucidchart or Draw.io          |
|             | - [x] Install Terraform and GitLab CI/CD tools                                                      |
|             | - [x] Initialize a new GitLab repository for the project                                            |
| **Day 2**   | **Code API, API (Docker containerisation and Set Up GitLab CI/CD Pipeline**                      |
|             | - [x] Develop a simple API using a language/framework of your choice                                 |
|             | - Write unit test for the API                                                                     |
|             | - [x] Plan Docker integration for API containerization.                                             |
|             | - [x] Identify necessary scripts for Docker image creation.                                         |
|             | - [x] Create necessary scripts (build, test, deploy) for the CI/CD pipeline                         |
|             | - [x] Configure `.gitlab-ci-cd.yml` for automated testing and deployment                                |
| **Day 3**   | **Infrastructure Setup with Terraform**                                                        |
|             | - Define infrastructure requirements (e.g., VPC, Subnets, Security Groups) using Terraform     |
|             | - Create Terraform files for AWS service configurations.         |
| **Day 4**   | **AWS Configuration and Deployment and Docker Implementation**                                      |
|             | - Start Docker implementation for API containerization.                                          |
|             | - Apply Terraform configuration to create infrastructure on AWS                                 |
|             | - Configure AWS services (like EC2 or any other service) for hosting your API                   |
|             | - Test manually to ensure the deployed infrastructure is functional                             |
| **Day 5**   | **CI/CD Testing and Refinement**                                                                |
|             | - Push code changes to GitLab and observe the CI/CD pipeline in action                           |
|             | - Debug and refine the pipeline as needed (handling errors, improving tests)                     |
|             | - Configure GitLab CI/CD with testing stages.                                                      |
|             | - Test Docker containerization and basic API functionality.                                       |
| **Day 6**   | **Documentation and Finalization**                                                              |
|             | - Document the project: Docker or Infrastructure setup, CI/CD workflow, and any troubleshooting steps       |
|             | - Review the project to ensure completeness and functionality                                   |
|             | - Prepare a demo or presentation to showcase your project                                        |
| **Day 7**   | **Presentation and Wrap Up**                                                                   |
|             | - Practice your demo/presentation                                                                |
|             | - Present your project to colleagues, mentors, or peers                                          |
|             | - Reflect on your learnings and note areas for improvement                                       |


## Tips for a Junior DevOps Engineer:

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
6. How will Docker be integrated for API containerization?
   - Use Docker to containerize the API for simplified deployment.

**Scope: Define the boundaries of your project. For example:**
1. Which parts of AWS will you use? (Avoid making it too complex at first)
   - AWS Components: Focus on using AWS Lambda and API Gateway for initial setup.
  - Utilize AWS Lambda and API Gateway
2. What level of complexity will your API have? (Start with a simple one and maybe add features later)
  - Begin with a simple API 
3. What specific tasks will you perform with Terraform and GitLab CI/CD? (Setting up infrastructure, automating testing and deployment)
- Terraform: Network and server setup; GitLab CI/CD: Automation of testing and deployment

**Constraints and Resources: Consider any limitations or resources available to you:**
1. Time: Two week to complete this project.
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
| Docker              | -                                    |                                                      |

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

3. **Docker Integration:**

Containerize the API using Docker for deployment.

4. **GitLab CI/CD:**
   - **Pipeline Configuration:** Contains stages for testing and deployment.
   - **Testing Steps:** Runs automated tests on the code.
   - **Deployment Steps:**
   - Builds Docker containers for the API.
   - Pushes the containerized code changes to AWS services using Terraform.

5. **Workflow Overview:**
   - Developer pushes code changes to GitLab repository.
   - GitLab CI/CD pipeline triggers.
   - Pipeline runs tests on the code.
   - Upon successful tests, Terraform applies changes to AWS infrastructure.
   - Docker containerization process wraps the updated code into containers.
   - Deploy the containerized code to Lambda via GitLab CI/CD, incorporating Docker into the deployment process for Lambda.

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
   - Docker Containerization
   - Code Deployment to Lambda
```


## Connect your laptop to GitLab using SSH, you'll need to follow these general steps:

1. **Generate SSH Key Pair:**
    - Open your terminal or command prompt on your laptop.
    - Use the command `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"` to generate a new SSH key pair. Replace `"your_email@example.com"` with the email address associated with your GitLab account.
    - It will prompt you to save the key in a specific file. Press Enter to save it in the default location (`~/.ssh/id_rsa`) or specify a different location.

2. **Add SSH Key to SSH-Agent (Optional but recommended):**
    - Start the SSH agent by running `eval "$(ssh-agent -s)"`.
    - Add your SSH private key to the SSH agent with `ssh-add ~/.ssh/id_rsa`.

3. **Add SSH Public Key to GitLab:**
    - Copy your SSH public key to the clipboard. You can do this by running `cat ~/.ssh/id_rsa.pub` and copying the output.
    - Log in to your GitLab account.
    - Go to `Settings > SSH Keys` and paste your SSH public key into the "Key" field.
    - Give the key a descriptive title and click on "Add key".

4. **Test the SSH Connection:**
    - In your terminal, run `ssh -T git@gitlab.com` (replace `git@gitlab.com` with your GitLab instance if using self-hosted GitLab).
    - If prompted to continue connecting, type `yes`.
    - If everything is set up correctly, you should see a message like `Welcome to GitLab, @your_username!`.

Now, your laptop should be connected to GitLab via SSH, allowing you to push, pull, or interact with repositories using SSH authentication.


## Brief guide on how to use the API:

### Endpoints:

#### 1. `/public_apis`:
   - **Method:** GET
   - **Purpose:** Retrieves a list of public APIs with optional filtering, searching, and sorting capabilities.
   - **Parameters:**
     - `category` (Optional): Filter APIs by category. Example: `/public_apis?category=Science`
     - `https` (Optional): Filter APIs by HTTPS support. Example: `/public_apis?https=true`
     - `search` (Optional): Search for specific APIs by keyword. Example: `/public_apis?search=weather`
     - `sort_by` (Optional): Sort the results by a specific field. Example: `/public_apis?sort_by=API`

#### 2. `/secure_public_apis`:
   - **Method:** GET
   - **Purpose:** Provides access to the `/public_apis` endpoint with authentication.
   - **Authentication:** Basic Authentication (username and password required).

### Usage Examples:

1. **Fetching all public APIs:**
   - Endpoint: `/public_apis`
   - Example URL: `http://yourdomain.com/public_apis`
   - Result: Retrieves a list of all available public APIs.

2. **Filtering by category:**
   - Endpoint: `/public_apis`
   - Example URL: `http://yourdomain.com/public_apis?category=Science`
   - Result: Retrieves a list of APIs categorized under 'Science'.

3. **Filtering by HTTPS support:**
   - Endpoint: `/public_apis`
   - Example URL: `http://yourdomain.com/public_apis?https=true`
   - Result: Retrieves a list of APIs that support HTTPS.

4. **Searching for specific APIs:**
   - Endpoint: `/public_apis`
   - Example URL: `http://yourdomain.com/public_apis?search=weather`
   - Result: Retrieves a list of APIs containing 'weather' in their names.

5. **Sorting the results:**
   - Endpoint: `/public_apis`
   - Example URL: `http://yourdomain.com/public_apis?sort_by=API`
   - Result: Retrieves a sorted list of APIs based on their names.

6. **Accessing secure endpoint with authentication:**
   - Endpoint: `/secure_public_apis`
   - Example URL: `http://yourdomain.com/secure_public_apis`
   - Authentication: Requires valid username and password via Basic Auth.

Remember to replace `http://yourdomain.com` with the actual domain where the Flask app is hosted and adjust parameters as needed.



## Getting Started

- Make sure you have Docker installed on your system.
- Open a terminal, navigate to the directory containing the Dockerfile and your Flask application files.

#### 1. Project Structure

This project has the following structure:

```
project_directory/
│
├── app.py
├── requirements.txt
├── Dockerfile
└── (other_files_and_folders)
```

- `app.py`: Flask application code.
- `requirements.txt`: File containing Python dependencies.
- `Dockerfile`: Configuration file for building the Docker image.

#### 2. Dockerfile Configuration

The `Dockerfile` should contain the following instructions:

```Dockerfile
# Use an official Python runtime as a base image
FROM python:3.9

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed dependencies specified in requirements.txt
RUN pip install -r requirements.txt

# Set environment variables, if needed
# ENV VARIABLE_NAME value

# Expose the port your app runs on
EXPOSE 5000

# Define the command to run your application
CMD ["python", "app.py"]
```

### Building the Docker Image

1. Open a terminal and navigate to the project directory containing the `Dockerfile`.
2. Run the following command to build the Docker image:

   ```bash
   docker build -t your_image_name:tag .
   ```

   Replace `your_image_name:tag` with your desired image name and tag.

### Running the Docker Container

Once the image is built successfully, start a container from it:

```bash
docker run -p 5000:5000 your_image_name:tag
```

Access the API at `http://localhost:5000`.

