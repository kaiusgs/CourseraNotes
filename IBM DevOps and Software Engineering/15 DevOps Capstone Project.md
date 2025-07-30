# DevOps Capstone Project  
## Brief  
In this Capstone project, you will apply many of the technologies and concepts you've learned in the preceding courses to build a Customer Accounts microservice.

Starting in Module 1, lesson 2 you will begin this capstone adventure by developing an Agile plan to create a RESTful microservice. You will create a GitHub repository and Kanban board to manage the project by building a user story template in GitHub to write well-structured user stories.  You will build a product backlog on your Kanban board by adding user stories to represent each step needed to build the Customer Accounts microservice. After finishing your product backlog, you will build a sprint plan. This step involves scheduling sprints, designating estimated story points to stories, assigning several stories to the next sprint, and building your sprint backlog. For every module, you will be directed to take screenshots and note the URLs in your GitHub repository. 

In module 2, lesson 1, you will begin sprint one by configuring the capstone project environment and developing the Customer Account microservice using test-driven development (TDD). As you work on each story, you will move the story through the kanban; from “backlog” to “In progress,” to “Done,” and finally, to “Closed.” 

For sprint 1, you will start developing a new branch on your GitHub repo, which you may subsequently push to the main branch by submitting pull requests at each point.     

You will create test cases for the read, update, delete, and list functions for a RESTful Flask service, and write enough code for the tests to pass. As you develop, you will run nosetests to ensure that all unit tests pass, and use the coverage tool to ensure that there is at least 95% coverage.  

In the next module, you will begin the sprint by configuring a GitHub Actions workflow that is triggered when an event occurs in the repository, such as whenever a pull request is created to the main branch or whenever a push happens to the main branch. Also, as part of sprint 2, you will create a workflow that builds and tests every push/pull request to your repository.  You will use Flake8 to lint your code, add quality checks to your CI pipeline, and configure nosetests to test the code coverage.  

In the next lesson, you will add secure code practices for the microservice you built by adding Flask-Talisman for security headers and Flask-CORS to establish Cross-Origin Resource Sharing (CORS) policies. To align with the TDD practices, you will write a test case for the security feature you are trying to implement. The failing test case should eventually pass once you include the code for adding security headers and CORS policies. Once you have added Flask Talisman for Security Headers and Flask-CORS to establish CORS policies, you will merge your branch with the main or master branch. 

In Sprint 3, module 4, you will work on two user stories sequentially. This involves creating a Docker image of your microservice and manually deploying the same to an OpenShift/ Kubernetes cluster. You will create a Dockerfile and use it to build an image called “accounts.” You will push this image to the IBM Cloud Container Registry and use this image to deploy to Kubernetes/OpenShift. For the second user story, the first task includes creating a PostgreSQL service in OpenShift, which serves as the database in Kubernetes for your application. You will move on to creating manifest YAML files for deploying the Docker image to the OpenShift cluster. For every story, you will continue to commit changes, push them, and then pull them into the main branch. 

For module 4, you will automate the deployment to Kubernetes using a Tekton pipeline so that when the pipeline is triggered, the accounts service will be deployed to Kubernetes without requiring manual intervention. You will create a CD pipeline, involving tasks for cloning, linting, unit testing, building, and deploying the service to an OpenShift/Kubernetes cluster. 

Module 5 is where you organize and submit your work for peer review. You will be required to review at least one of your peers’ projects using the provided rubric which describes the number of points that should be awarded for task completion, partial completion, or not completed. 

Good Luck! 