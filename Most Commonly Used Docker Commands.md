

### **Most Commonly Used Docker Commands**

| **Category**         | **Command**               | **Purpose**                                                                                   | **Example**                                                                 |
|-----------------------|---------------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **⚙️ System Commands** | `docker system df`        | Show disk usage for images, containers, and volumes. 📊                                        | `docker system df`                                                         |
|                       | `docker system prune`     | Remove unused data (stopped containers, networks, dangling images, build cache). 🗑️           | `docker system prune -a`                                                   |
|                       | `docker system info`      | Display system-wide information (e.g., number of containers, images, etc.). 🌟                | `docker system info`                                                       |
| **📦 Container Commands** | `docker run`            | Create and start a new container from an image. 🚀                                            | `docker run -d -p 80:80 nginx`                                             |
|                       | `docker ps`              | List running containers. 📋                                                                   | `docker ps`                                                                |
|                       | `docker ps -a`           | List all containers (including stopped ones). 📜                                              | `docker ps -a`                                                             |
|                       | `docker start`           | Start a stopped container. ▶️                                                                 | `docker start <container_id>`                                              |
|                       | `docker stop`            | Stop a running container gracefully. ⏹️                                                       | `docker stop <container_id>`                                               |
|                       | `docker rm`              | Remove one or more containers. 🗑️                                                            | `docker rm <container_id>`                                                 |
|                       | `docker exec`            | Run a command inside a running container. 💻                                                  | `docker exec -it <container_id> bash`                                      |
|                       | `docker logs`            | View logs of a container. 📝                                                                  | `docker logs <container_id>`                                               |
|                       | `docker stats`           | Display live resource usage statistics for containers. 📈                                     | `docker stats`                                                             |
| **🖼️ Image Commands**    | `docker images`          | List locally stored images. 📂                                                               | `docker images`                                                            |
|                       | `docker pull`            | Pull an image from a registry (e.g., Docker Hub). 📥                                          | `docker pull nginx`                                                        |
|                       | `docker push`            | Push an image to a registry. 📤                                                              | `docker push myrepo/myimage:tag`                                           |
|                       | `docker build`           | Build an image from a Dockerfile. 🛠️                                                          | `docker build -t myimage:tag .`                                            |
|                       | `docker rmi`             | Remove one or more images. 🗑️                                                                | `docker rmi <image_id>`                                                    |
|                       | `docker tag`             | Tag an image for a repository. 🏷️                                                             | `docker tag <image_id> myrepo/myimage:tag`                                 |
| **🌐 Network Commands**   | `docker network ls`      | List networks. 📊                                                                             | `docker network ls`                                                        |
|                       | `docker network create`  | Create a new network. 🌟                                                                      | `docker network create mynetwork`                                          |
|                       | `docker network inspect` | Inspect a network. 🔍                                                                         | `docker network inspect bridge`                                           |
|                       | `docker network rm`      | Remove a network. 🗑️                                                                         | `docker network rm mynetwork`                                              |
| **💾 Volume Commands**    | `docker volume ls`       | List volumes. 📂                                                                              | `docker volume ls`                                                         |
|                       | `docker volume create`   | Create a new volume. 🆕                                                                       | `docker volume create myvolume`                                            |
|                       | `docker volume rm`       | Remove a volume. 🗑️                                                                          | `docker volume rm myvolume`                                                |
| **🔗 Compose Commands**   | `docker-compose up`      | Start and attach to containers defined in a `docker-compose.yml` file. 🚀                     | `docker-compose up -d`                                                     |
|                       | `docker-compose down`    | Stop and remove containers, networks, and volumes defined in a `docker-compose.yml` file. 🗑️ | `docker-compose down`                                                      |
|                       | `docker-compose ps`      | List containers managed by Docker Compose. 📋                                                | `docker-compose ps`                                                        |
|                       | `docker-compose logs`    | View logs of services defined in a `docker-compose.yml` file. 📝                              | `docker-compose logs`                                                      |
| **✨ Miscellaneous**      | `docker version`         | Show Docker version information. 📜                                                           | `docker version`                                                           |
|                       | `docker info`            | Display system-wide information (e.g., number of containers, images, etc.). 🌟               | `docker info`                                                              |
|                       | `docker login`           | Log in to a Docker registry. 🔑                                                              | `docker login`                                                             |
|                       | `docker logout`          | Log out from a Docker registry. 🚪                                                            | `docker logout`                                                            |
|                       | `docker search`          | Search for images on Docker Hub. 🔍                                                          | `docker search nginx`                                                      |
|                       | `docker cp`              | Copy files/folders between a container and the local filesystem. 📥                           | `docker cp <container_id>:/path/to/file /local/path`                       |

---

### **📚 Key Notes**
1. Replace placeholders like `<container_id>`, `<image_id>`, and `<network_name>` with actual values. 📝
2. Use `-d` for detached mode when running containers. 🚀
3. Use `-it` for interactive terminal access when using `docker exec`. 💻
4. Use `--help` after any command for additional options. Example: `docker run --help`. ❓

---
### for more info read docker docs
