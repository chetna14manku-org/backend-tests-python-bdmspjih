# Trusted Application Pipeline Software Template

This application, **backend-tests-python-bdmspjih**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/chetna14manku-org/backend-tests-python-bdmspjih ](https://github.com/chetna14manku-org/backend-tests-python-bdmspjih ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/chetna14manku-org/backend-tests-python-bdmspjih-gitops ](https://github.com/chetna14manku-org/backend-tests-python-bdmspjih-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |
| **demo-app-ci** | The namespace used for CI workloads |
| **demo-app-development** | The default application during development. Every build will be deployed to this namespace for testing. |
| **demo-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/chetna14manku-org/backend-tests-python-bdmspjih-gitops ) in the components/backend-tests-python-bdmspjih/overlays/stage directory |
| **demo-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/chetna14manku-org/backend-tests-python-bdmspjih-gitops ) in the components/backend-tests-python-bdmspjih/overlays/prod directory |