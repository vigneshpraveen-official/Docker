# 🚀 Essential Docker Commands Cheat Sheet

## 🔹 General Commands
| Command | Description |
|---------|------------|
| `docker --version` | Check installed Docker version |
| `docker info` | Display system-wide information about Docker |
| `docker help` | Get help for Docker commands |

## 🚀 Working with Images
| Command | Description |
|---------|------------|
| `docker pull <image>` | Download an image from Docker Hub |
| `docker images` | List all available images on the system |
| `docker rmi <image>` | Remove an image from the system |

## 📦 Container Management
| Command | Description |
|---------|------------|
| `docker run <image>` | Create and run a new container from an image |
| `docker run -d <image>` | Run a container in **detached mode** (background) |
| `docker run -it <image> bash` | Run a container in **interactive mode** with Bash shell |
| `docker ps` | List running containers |
| `docker ps -a` | List **all** containers (including stopped ones) |
| `docker stop <container_id>` | Stop a running container |
| `docker start <container_id>` | Start a **stopped** container |
| `docker restart <container_id>` | Restart a container |
| `docker rm <container_id>` | Remove a container |
| `docker logs <container_id>` | View logs of a running container |

## 💻 Container Interaction
| Command | Description |
|---------|------------|
| `docker exec -it <container_id> bash` | Access a running container’s shell |
| `docker attach <container_id>` | Attach to a running container’s console |
| `docker inspect <container_id>` | Get detailed information about a container |

## 🔨 Building Images
| Command | Description |
|---------|------------|
| `docker build -t <image_name> .` | Build an image from a Dockerfile |
| `docker tag <image> <repo>:<tag>` | Tag an image for pushing to a repository |

## 🌐 Networking
| Command | Description |
|---------|------------|
| `docker network ls` | List all Docker networks |
| `docker network create <network_name>` | Create a custom Docker network |
| `docker network inspect <network_name>` | View details of a network |
| `docker network connect <network> <container>` | Connect a container to a network |

## 💾 Volumes & Data Persistence
| Command | Description |
|---------|------------|
| `docker volume create <volume_name>` | Create a Docker volume |
| `docker volume ls` | List all volumes |
| `docker volume inspect <volume_name>` | View volume details |
| `docker run -v <volume_name>:/path <image>` | Mount a volume to a container |

## 🛠️ Docker Compose
| Command | Description |
|---------|------------|
| `docker-compose up -d` | Start all services in a `docker-compose.yml` file |
| `docker-compose down` | Stop and remove all services |
| `docker-compose ps` | List services managed by Docker Compose |

## 🗑️ Cleaning Up
| Command | Description |
|---------|------------|
| `docker system prune` | Remove unused containers, networks, images, and volumes |
| `docker container prune` | Remove **all stopped containers** |
| `docker image prune` | Remove **unused** images |
| `docker volume prune` | Remove **unused** volumes |

---

## 📌 Notes:
- `<container_id>` and `<image>` refer to actual **container IDs** and **image names**.
- Use `docker ps -q` to get only container IDs and `docker images -q` for image IDs.
- Running `docker rm $(docker ps -aq)` removes **all containers** at once.
- Running `docker rmi $(docker images -q)` removes **all images**.

---

🔥 **This cheat sheet provides essential Docker commands for beginners and professionals.**  
💡 *Star ⭐ this repository if you find it helpful!*  

