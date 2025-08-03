# DevOps Capstone Project  
> **Customer Accounts microservice**
## Sprint0 
- Create a GitHub repository  
- Create a GitHub kanban board  
- Develop a user story template  
- Add user stories to the kanban board  
    - and Triage New Issues  
- Sort user stories to prepare for backlog refinement  
- Refine a product backlog to make it sprint ready  
    - move all remaining unsorted stories into appropriate pipelines, add sufficient detail to each story, and label each story appropriately.  
- Build a sprint plan  
    - scheduling sprints(set sprints iteration), designating estimated story points to stories, assigning several stories to the next sprint, and building your sprint backlog.  
## Sprint1
- general workflow:  
    - Get the next highest-ranked story to work on.  
    - Create a branch to work in.  
    - Implement a test case that asserts the correct behavior.  
    - Implement the code to make the test case pass.  
    - Maintain code coverage of 95% or better.  
    - Make a pull request to merge your changes.  
        - ```git push --set-upstream origin {your branch name}``` push the changes along with the new-created branch  
    - Update the kanban board by moving your story to Done.  
## Sprint2  
- Part1  
    - Create a GitHub Actions workflow to run your CI pipeline  
        - Create a GitHub Actions workflow in the `.github/workflows` folder of your GitHub repository called `ci-build.yaml`  
    - Add events to trigger the workflow  
    - Add a job to the workflow  
    - Add steps to a job  
    - Run inline commands in the steps  
        - A GitHub Actions badge should be added the README.md to reflect the build status:  
        ```![Build Status](https://github.com/<OWNER>/<REPOSITORY>/actions/workflows/<WORKFLOW_FILE>/badge.svg)```  
    - Review the logs for a workflow run  
    - View the activity for a workflow run  
- Part2  
    - add secure code practices to the RESTful service: Talisman, CORS  
## Sprint3  
- At first, you will find your user story "Containerize your microservice using Docker" in the kanban board, move it to "In Progress," and assign it to yourself. 
- Next, you will create the Dockerfile and then use it to build to Docker image called "accounts." You will push this image to the IBM Cloud Container Registry. 
- You will use this image to deploy to Kubernetes/OpenShift as part of the "Deploy your Docker image to Kubernetes" user story.  
    - Create Kubernetes manifests for your deployment
    - Deploy your Docker image in an OpenShift Kubernetes cluster
    - View the logs to ensure your service is running
    - Make a pull request and merge your changes
    - Move the story to Done
- For your second user story, the first task will include creating a PostgreSQL service in OpenShift, which will serve as the database in Kubernetes for your application. 
- You will move on to creating manifest YAML files for deploying the Docker image to the OpenShift cluster.  
> Automate the deployment to Kubernetes using the Tekton pipeline so that when the pipeline is triggered, the accounts service will be deployed to Kubernetes without requiring any manual intervention. 

- To start, you will find the user story "Create a CD pipeline to automate deployment to Kubernetes" in the kanban board, move it from the "Sprint Backlog" to "In Progress," and assign it to yourself.  
- Next, you will create the CD pipeline, involving tasks for cloning, linting, unit testing, building, and deploying the service to an OpenShift/Kubernetes cluster.  

| Task Name | Build After | Message |
| - | - | - |
| clone | - | Cloning the repo $(params.repo-url) |
| lint | clone | Calling Flake8 linter| 
| tests | clone | Running unit tests with PyUnit| 
| build | lint, tests | Building image for $(params.repo-url)| 
| deploy | build | Deploying $(params.branch) branch of $(params.repo-url)| 