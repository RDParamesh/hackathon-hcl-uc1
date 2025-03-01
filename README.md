# Assignment for Cloud/DevOps
## Objective
Demonstrate your capability in cloud engineering by completing the following tasks.
## Create a GitHub Repository
Name the repository as you see fit.
The repository can be either private by forking the Git Repo.If private, please grant user SubbuHCL read access.
## Develop a Simple API Application:
Create a API application that returns "Hello, World!" on the API which using NodeJS as an API.
Ensure the application is internet-facing and JWT Authentication.
Use the code available in backend, but preference will be given to serverless solutions rather than virtual machines.
## Set Up a CI/CD Pipeline:
Automate the deployment process of your application to AWS.
Choose a hosting service of your preference (e.g., AWS Lambda, S3,API Gateway, etc.).
Use any CI/CD tool ( GitHub Actions) to set up the pipeline.
## Documentation:
Add a README file to your repository that includes:
An architecture diagram of your application.
A detailed explanation of the steps executed in your CI/CD pipeline.
Instructions on how to test and verify the application.

Architecture: 

Infrastructure: 

VPC—IGW---Subnets——Routetable—Subnetassociation——security-group—ECR deployment in this VPC  am creating by using vpc module.


IAM roles— Assumerolewithwebidentity—for gitlab to aws authentication

IAM roles to fetch the image from ECR

Docker file need to write

CICD—stages—cloning the repo—authenticate to ECR—aws login with assume role with web identiy---build the image and push it ECR—deploy to ECS
