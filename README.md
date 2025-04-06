#  **Module: Containerization with Docker – Build, Ship, Run Anywhere**

1.  Introduces the **Docker module** in context of what learners have already completed  
2.  Covers the **entire Docker module** content in one clean flow  
3.  References **Jenkins Section 7**, explaining which parts are covered here  
4.  Lays the groundwork for future Kubernetes modules  

---
---

##  **Introduction**

Till this point in your DevOps journey, you’ve already mastered some essential building blocks:

- **Version control** with Git and GitHub  
- **Build automation tools** like Maven, npm, and pip  
- The **core concepts of CI/CD**  
- And hands-on automation using **Jenkins**

Now imagine this…

You’ve built a Java or Node.js app. Jenkins is building and testing it perfectly on your EC2 instance. But when you move it to another machine — it breaks.

Why?

- Different OS  
- Missing dependencies  
- Configuration mismatch  

This is where **Docker** enters.

Docker allows you to **package your application with everything it needs** — OS libraries, dependencies, runtime — into a single image that **runs consistently everywhere**.

In this module, we’ll also cover **parts of Jenkins Section 7**, specifically:

- Building Docker images using Jenkins  
- Pushing images to Docker Hub  
- Running containers in a Jenkins CI/CD pipeline  

> We will **not cover Kubernetes** here. Once you complete this module, you’ll be ready to move into Kubernetes and then revisit Jenkins Section 7 for full CI/CD to Kubernetes.

---

##  **Module Objective**

To help learners understand what containers are, how Docker works, and how to build, run, manage, and ship containerized applications in real-world DevOps pipelines.

---

#  **Course Content**

---

## Section 1 – Introduction to Containers and Docker

- What is containerization and why we need it  
- Virtual Machines vs Containers  
- Benefits of containers for DevOps and CI/CD  
- Docker architecture and components  
  - Docker Engine, Client, Daemon, Images, Containers  
- Install Docker on Ubuntu or EC2  
- Lab: Install Docker and run hello-world container  

---

## Section 2 – Docker Images and Containers

- What is a Docker image  
- What is a Docker container  
- Lifecycle: create, run, pause, stop, delete  
- Docker Hub and public images  
- Lab:  
  - Pull and run NGINX container  
  - Explore `docker ps`, `docker run`, `docker logs`, `docker stop`

---

## Section 3 – Writing and Building Dockerfiles

- What is a Dockerfile  
- Step-by-step breakdown of a Dockerfile  
- Instructions: FROM, RUN, COPY, CMD, ENTRYPOINT, EXPOSE  
- Lab:  
  - Write Dockerfile for Node.js or Python app  
  - Build and tag image  
  - Run container and access app  
- Best practices for Dockerfile design  

---

## Section 4 – Docker Container Management

- Docker image and container CLI commands  
  - docker ps, stop, start, rm, exec, logs  
- Container resource limits  
- Setting environment variables  
- Port mapping  
- Lab:  
  - Run a web app with port exposed and env variables  
  - Connect to the container and test inside shell  

---

## Section 5 – Docker Storage: Volumes and Bind Mounts

- Why containers need persistent storage  
- Volume types  
  - Anonymous  
  - Named  
  - Bind mounts  
- Lab:  
  - Create named volume  
  - Attach to container  
  - Persist MySQL or logs  
  - Inspect, remove, and reuse volumes  
- Real-world example:  
  - Store uploads or DB data across container restarts  

---

## Section 6 – Docker Compose

- What is Docker Compose and why it’s useful  
- YAML file structure: version, services, volumes, ports  
- Lab:  
  - Multi-container app with Node.js and MongoDB  
  - Build and run with `docker-compose up`  
  - Rebuild with changes, tear down with `docker-compose down`  

---

## Section 7 – Docker Networking and Troubleshooting

- Docker network types  
  - Bridge  
  - Host  
  - None  
- Connecting containers via custom networks  
- Lab:  
  - Create isolated bridge network  
  - Run multiple containers and ping each other  
- Troubleshooting common issues:  
  - Port conflicts  
  - Permissions  
  - Stuck containers  

---

## Section 8 – Docker in CI/CD with Jenkins (Jenkins Section 7.2 and 7.5)

- Use Jenkins to build and push Docker image  
- Docker login using Jenkins credentials  
- Jenkinsfile for Docker build pipeline  
- Lab:  
  - Jenkins builds Docker image for a Node app  
  - Push image to Docker Hub  
  - Deploy container on same EC2 or test VM  
- Prepares for: Jenkins to Kubernetes in next module  

---

## Section 9 – Docker Registries and Image Management

- What is Docker Hub  
- Public vs private repositories  
- Tagging images  
- Push and pull from registry  
- Brief on ECR and GCR  
- Lab:  
  - Tag and push image to Docker Hub  
  - Pull and run on another server  

---

## Section 10 – Docker Swarm – Lightweight Orchestration (Optional)

> This is a **teaser** for Kubernetes orchestration. Meant for understanding orchestration basics.

- What is Docker Swarm  
- Swarm architecture: Manager and Worker nodes  
- Creating and joining Swarm  
- Lab:  
  - Initialize a Swarm on single-node  
  - Deploy a service  
  - Scale up and down  
  - Update container without downtime  
- When to use Swarm vs when not  

---

## Section 11 – Containerizing Real-World Applications

- Lab 1: Containerize a Java Maven web app  
- Lab 2: Containerize a Node.js app with environment variables  
- Lab 3: Add Docker Compose with DB  
- Push to registry  
- Share with team  

---

## Section 12 – Bonus and Troubleshooting

- .dockerignore usage  
- Debugging with docker exec and logs  
- Reducing image size  
- Clean-up: system prune, unused images, volumes  
- Real-world errors and how to fix them

---

##  What Comes Next

Once learners complete this module, they are now ready to:
- Learn **Kubernetes and container orchestration** in depth  
- Complete **Jenkins Section 7** with Docker and Kubernetes pipelines  
- Handle **CI/CD for modern cloud-native applications** end to end  

---
---

