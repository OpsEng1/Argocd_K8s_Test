# Testing a Kubernetes Deployment on ArgoCD

This is a simple repo to test the Kubernetes repo section on ArgoCD

To create a simple application, click on "new app" and "edit as yaml". Copy the code in the argo_application.yaml file and click create.

The application should run with the same numebr of replicas mentioned in the deployment.yaml file. When you try to manually scale the number of replicas from command line, you will see the same number of pods spun up on ArgoCD but eventually since "SelfHeal" is set to true, the configuration will "correct" itself to reflect what is in the github files. 

As an additonal test, increase the number of replicas in the deployment file and this will reflect accordingly on ArgoCD. Click on the events tab of the application to see what is happening.

Happy Learning!
