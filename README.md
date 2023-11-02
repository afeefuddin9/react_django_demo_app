# react_django_demo_app
Deploying a Django Application on AWS EC2 with Docker🐳
# Deploy Netflix Clone on Cloud using Manual way & Jenkins - DevOps Project!

### **Phase 1: Initial Setup and Deployment**
1. An AWS account
2. Install Docker machine
3. Install Docker-Compose
4. Clone the Django application

**Clone the Code:**

- Update all the packages and then clone the code.
- Clone your application's code repository onto the EC2 instance:
    
    ```markdown
    git clone https://github.com/afeefuddin9/react_django_demo_app.git
    ```

Steps
**Dockerize your Django application**

**Create a Dockerfile for your Django application. This file will define the steps that Docker will take to build and run your application.**

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696316589125/838ceb79-0fc9-484d-a0a8-0a0ff9f7aff5.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

**Build your Docker image.**

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317312598/0f44244e-be5d-421e-962e-1845ef380f8f.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

**Push your Docker image to a Docker registry, such as AWS ECR or you can store it locally on ec2 itself.**

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317951723/83ab10d8-3391-4d26-a031-6bd20fce0887.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

**Deploy your Django application to AWS EC2**

Launch an EC2 instance.

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317634415/4e5f6a38-7b0c-4709-9802-24fabe06b512.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317652792/85c329a1-f4b1-4050-8e45-400fb3a89720.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317665480/b02ca733-d329-40d8-a703-22a00b8aac5f.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317676145/c49d4895-cdde-485c-b9d8-2119b0f2c1db.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317692032/a563fd9e-df0a-4296-9c1b-1168da358674.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

<div class="image-div">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317738652/65b01dfb-82c4-48a4-9e6c-985076b02064.png?auto=compress,format&format=webp" alt="Image" width="auto">
</div>

**Install Docker on the EC2 instance.**

**Steps to Install Docker: Install Docker and Run the App Using a Container:**

- Set up Docker on the EC2 instance:

```bash
sudo apt-get update
sudo apt-get install docker.io -y
sudo usermod -aG docker $USER  # Replace with your system's username, e.g., 'ubuntu'
newgrp docker
sudo chmod 777 /var/run/docker.sock
```

<div class="image-div" style= "margin-top: 2em; margin-bottom: 2em;">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317799695/6c8c7c52-c4e7-4c2a-91aa-0e2ae1b25aa3.png?auto=compress,format&format=webp" alt="Image" width="90%">
</div>

**Pull your Docker image from the Docker registry or Run the container from the image that you have created locally.**

<div class="image-div" style= "margin-top: 2em; margin-bottom: 2em;">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696317958590/57c8e4d4-a3b9-4630-b42c-67f5bcdc7abc.png?auto=compress,format&format=webp" alt="Image" width="90%">
</div>

**Run your Docker image on the EC2 instance.**

<div class="image-div" style= "margin-top: 2em; margin-bottom: 2em;">
  <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1696318027765/b6639ffc-9fd7-465c-94e8-a782f6e44690.png?auto=compress,format&format=webp" alt="Image" width="90%">
</div>
```

In the above code, I wrapped each image in a `<div>` with the class "image-div" and added a `padding-bottom` to create space. You can further style this class in a separate CSS section or file if needed.

This will add space after each image section in your `README.md` file.
