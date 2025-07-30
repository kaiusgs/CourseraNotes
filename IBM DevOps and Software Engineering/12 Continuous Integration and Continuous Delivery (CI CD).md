# Continuous Integration and Continuous Delivery (CI CD)  
## CI CD  
- Continuous Integration is an automation process that allows developers to continuously integrate their code back into the main or master branch.  
- Continuous Delivery is the next phase after CI, that takes integrated code and deploys it somewhere like a staging, testing, or preproduction server.  
- Continuous Deployment is delivering the code to production.  
![ci_cd](./static/12/ci_cd.png)  
![continuous_deployment](./static/12/continuous_deployment.png)  
- Infrastructure as Code  
    - An approach in which infrastructure configuration and management are automated using code.  
    - IaC tools can speed up the process of provisioning the development environment’s infrastructure.  
    ![inventory_files_&_iac_tools](./static/12/inventory_files_&_iac_tools.png)  
## Continuous Integration  
- Main features  
    - short-lived branches  
    - frequent pull requests  
    - automated CI tools  
- Social Coding  
![social_coding_steps](./static/12/social_coding_steps.png)  
- CI Pipeline: The CI pipeline validates, packages, and builds essential components, creating deployable artifacts like container images and helm charts. It ensures versioning and resource preparation.
- Git  
![git_common_command_flow](./static/12/git_common_command_flow.png)  
![before_pull_request](./static/12/before_pull_request.png)  
![after_pull_request](./static/12/after_pull_request.png)  
- Github Actions 
![github_actions_workflow](./static/12/github_actions_workflow.png)  
![event](./static/12/event.png)  
![jobs](./static/12/jobs.png)  
![runners](./static/12/runners.png)  
![services](./static/12/services.png)  
![steps](./static/12/steps.png)  
![actions](./static/12/actions.png)  
> Always check the *GitHub Actions Marketplace* for any action you may want to perform.  

![workflow_example](./static/12/workflow_example.png)  
## Continuous Delivery  
- A series of practices designed to ensure that code can be rapidly and safely deployed to production by delivering every change to a production-like environment.  
![cd_pipeline](./static/12/cd_pipeline.png)  
![ci_cd_pipeline_requirements](./static/12/ci_cd_pipeline_requirements.png)  
![cd_pipeline_tasks](./static/12/cd_pipeline_tasks.png)  
> - Dynamic Application Security Testing (DAST): Dynamic Application Security Testing (or DAST) scans for incorrect security assumptions hidden in the source code.  
> - Static Application Security Testing (SAST): Identifies vulnerabilities of the entire code base, such as SQL injections and cross-site scripting.  

- Tekton  
    ![tekton_building_blocks](./static/12/tekton_building_blocks.png)  
    - Tekton is a set of Kubernetes custom resource definitions, or CRDs.  
    - Pipeline, Tasks & Steps  
        - EventListeners listen for external events, TriggerBindings respond to those events and bind parameters from them, and TriggerTemplates create PipelineRuns that pass the parameters to the pipeline.  
        ![physical_building_blocks](./static/12/physical_building_blocks.png)  
        - Hello World Pipeline  
        ![helloworld_pipeline](./static/12/helloworld_pipeline.png)  
        ![task_example](./static/12/task_example.png)  
        ![pipeline_example](./static/12/pipeline_example.png)  
        > ![run_after](./static/12/run_after.png)  

        ![run_pipeline](./static/12/run_pipeline.png)  
    - Events & Triggers  
        ![tekton_triggers_flow](./static/12/tekton_triggers_flow.png)  
        ![eventlistener_example](./static/12/eventlistener_example.png)  
        ![triggerbinding_example](./static/12/triggerbinding_example.png)  
        ![triggertemplate_example1](./static/12/triggertemplate_example1.png)  
        ![triggertemplate_example2](./static/12/triggertemplate_example2.png)  
        ![parameter_flow](./static/12/parameter_flow.png)  
        ![trigger_the_pipeline](./static/12/trigger_the_pipeline.png)  
        > Error: unknown flag: --latest

        - `tkn pipelinerun ls` - list all the pipelinerun  
        - `tkn pipelinerun logs --last` - show the logs of the last pipelinerun 
    - Tekton Hub / Tekton Catalog  
        ![hub_tekton_dev](./static/12/hub_tekton_dev.png)  
        - ```tkn hub install task <name>``` - install the task from Tekton Hub  
        ![workspace](./static/12/workspace.png)  
        ![git_clone_example](./static/12/git_clone_example.png)  
    - Quality Check & Testing  
        ![testing_script](./static/12/testing_script.png)  
        ![define_the_task](./static/12/define_the_task.png)  
        ![add_database_uri_from_secret](./static/12/add_database_uri_from_secret.png)  
    - Build image  
        - ```tkn hub search --kinds task build``` - search image building task from Takton Hub  
        - ```tkn clustertask ls``` - list cluster level task that has been installed, making sure you don't have to install it locally into you namespace if it already exists.  
        - using a cluster-level installed task:  
            ![buildah](./static/12/buildah.png)  
    - Deploy  
        - ```tkn hub info task <task_name>``` - describe the information about the task.  
        ![deploy_task](./static/12/deploy_task.png)  
        ![alter_deploy_task](./static/12/alter_deploy_task.png)  
- **Continuous Compliance** pipeline ensures that organizations maintain security and compliance standards.  
- Openshift Pipelines  
![openshit_pipeline_main_concepts](./static/12/openshit_pipeline_main_concepts.png)  
- GitOps  
    - GitOps is a set of practices that use Git pull requests to manage infrastructure and application configurations.  
    - principles:  
        - Defines system definition as code.  
        - Versions and defines desired system configration.  
        - Provide GitChanges that enable pull requests.  
        - Offers a controller to avoid configration drifts.  
    - patterns on Openshift  
        - On-Cluster Resource Reconciler pattern  
        - External Resource Reconciler pattern  
