#   DevOps Project On Improving collaboration by integrating multiple tools #

# About # 
The DevOps  project  that simulates a typical DevOps workflow by integrating various tools for containerization, continuous integration (CI), continuous deployment (CD), and Kubernetes orchestration. The project is fully Dockerized, ensuring portability and ease of deployment across different environments.

# Tools Used #
- **Version Control:** Git + GitHub – For source code tracking and collaboration.
- **CI/CD Pipeline:** Jenkins – To automate the build, test, and deployment processes.
- **Containerization:** Docker – For packaging the backend into portable containers.
- **Container Orchestration:** Kubernetes (Minikube) – To manage and scale containers locally.
- **Code Quality**: SonarQube – For static code analysis to ensure code quality.
- **Node.js** – The core backend application, running on port 3000.


How to Run the Project (After Downloading)
# Prerequisites #
Make sure the following tools are installed:

- Docker: Install Docker
- Minikube: Install Minikube
- Kubectl: Install Kubectl
- Git: Install Git

# 🛠️ Step 1: Clone the Repository #

**Download the project from GitHub:**
- git clone https://github.com/your-username/your-repo.git
- cd your-repo

# 🐳 Step 2: Build and Push Docker Image #

 **Ensure Docker is running:**
- docker --version

 **Build the Docker image:**
- docker build -t yourdockerhubusername/devops-backend:1.0 .

 **Log in to Docker Hub:**
- docker login

 **Push the image to Docker Hub:**
- docker push yourdockerhubusername/devops-backend:1.0

# 📦 Step 3: Start Minikube #

 **Start Minikube:**
- minikube start

 **Verify the Minikube cluster is running:**
- kubectl get nodes

# 📜 Step 4: Deploy to Kubernetes #

 **Apply the Kubernetes configuration:**
- kubectl apply -f k8s-deployment.yml

 **Check if the pods are running:**
- kubectl get pods

# 🌐 Step 5: Access the Application #

 **Expose the service and get the URL:**
- minikube service backend-service
- Open the URL in your browser (e.g., http://192.168.xx.xx:xxxx).

# 📊 Step 6: Check Logs and Status #

 **Monitor the pod logs:**
- kubectl logs -f <pod-name>

 **If there are issues, describe the pod:**
- kubectl describe pod <pod-name>

# 🧹 Step 7: Clean Up #

 **When done, delete the deployment and stop Minikube:**
- kubectl delete -f k8s-deployment.yml
- minikube stop


# Jenkins #
![Screenshot 2025-03-06 015652](https://github.com/user-attachments/assets/70ee34fe-4d1b-420f-9bd5-ee3197ef2fea)

![Screenshot 2025-03-06 015634](https://github.com/user-attachments/assets/6ffa7509-cfa1-442b-90c6-59f1ae84fac4)

# Docker #
![Screenshot 2025-03-06 023331](https://github.com/user-attachments/assets/38ece7e5-5ca8-4e66-bea6-4213e0af89f6)

![Screenshot 2025-03-06 011128](https://github.com/user-attachments/assets/2c9bd26a-f403-43ff-89a3-bb6c44f07e24)

# Running Minikube #
![Screenshot 2025-03-06 021149](https://github.com/user-attachments/assets/18424a9c-e018-4ac1-b75d-fb55539f0e47)

![Screenshot 2025-03-06 022521](https://github.com/user-attachments/assets/fb12e353-4c8a-4476-ae9b-6c42cab063ae)









