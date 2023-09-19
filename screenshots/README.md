# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Website endpoint:
http://a7b280e2c349a466b9ffd0b38863e48e-1991614236.us-east-1.elb.amazonaws.com

## Deployment Pipeline
* DockerHub
  ![1](https://github.com/mei1011/AWS-project3/assets/136874890/7b1e66ff-9f60-408a-97a2-a369ea2bafa1)
  ![2](https://github.com/mei1011/AWS-project3/assets/136874890/66ce828a-b57d-4a4d-bfa9-14ed74459706)
  ![3](https://github.com/mei1011/AWS-project3/assets/136874890/bf79c2cc-103d-4387-8b2b-1f641e08b76f)
  ![4](https://github.com/mei1011/AWS-project3/assets/136874890/19044249-ff7f-48c8-8cef-3ddc8dfcbbf1)
  ![5](https://github.com/mei1011/AWS-project3/assets/136874890/6f118ef5-de55-4c24-9ef7-d899073a4d54)

* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook).

  **I used Github action instead of Travis. Because I had problems with my travis's account**

   Here are some of the main similarities between Travis CI and GitHub Actions:

  - Both tools use YAML (YAML Ain't Markup Language) format for their configuration files.
  - Both tools support a wide range of programming languages, such as Python, Ruby, Java, Node.js, and more.
  - Both tools allow you to run your workflows on different operating systems, such as Linux, Windows, and macOS.
    
**=>  Here is my workflows build.yml: https://github.com/mei1011/AWS-project3/blob/main/.github/workflows/build.yml**

* Travis CI showing a successful build and deploy job:
  
**=> Here is my action: https://github.com/mei1011/AWS-project3/actions**
  
## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![6](https://github.com/mei1011/AWS-project3/assets/136874890/0b5f3410-98a9-42cd-b4ce-3e089768578c)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![7](https://github.com/mei1011/AWS-project3/assets/136874890/17134b54-ea06-4f8b-90ed-1d65003fc50e)
![8](https://github.com/mei1011/AWS-project3/assets/136874890/1e3e91c3-6723-436f-a4d7-d29879fa5802)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![9](https://github.com/mei1011/AWS-project3/assets/136874890/cefeaf0b-cb4c-4ee0-a956-fb7b51b03a4b)

* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![10](https://github.com/mei1011/AWS-project3/assets/136874890/88847eba-10a7-455b-8cd2-323183db816d)
