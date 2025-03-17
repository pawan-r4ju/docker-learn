# Docker All Commands

## **Docker Command Categories**
1. **System Commands**
2. **Container Commands**
3. **Image Commands**
4. **Network Commands**
5. **Volume Commands**
6. **Docker Compose Commands**
7. **Miscellaneous Commands**


## **1. System Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker system df`  | Show disk usage for images, containers, and volumes.                                          | `docker system df`                                                         |
| `docker system prune` | Remove unused data (stopped containers, networks, dangling images, build cache).            | `docker system prune -a`                                                   |
| `docker system events` | Get real-time events from the Docker daemon.                                                | `docker system events`                                                     |
| `docker system info` | Display system-wide information (e.g., number of containers, images, etc.).                  | `docker system info`                                                       |

---

## **2. Container Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker run`        | Create and start a new container from an image.                                               | `docker run -d -p 80:80 nginx`                                             |
| `docker ps`         | List running containers.                                                                      | `docker ps`                                                                |
| `docker ps -a`      | List all containers (including stopped ones).                                                 | `docker ps -a`                                                             |
| `docker start`      | Start a stopped container.                                                                    | `docker start <container_id>`                                              |
| `docker stop`       | Stop a running container gracefully.                                                          | `docker stop <container_id>`                                               |
| `docker restart`    | Restart a running container.                                                                  | `docker restart <container_id>`                                            |
| `docker rm`         | Remove one or more containers.                                                                | `docker rm <container_id>`                                                 |
| `docker exec`       | Run a command inside a running container.                                                     | `docker exec -it <container_id> bash`                                      |
| `docker logs`       | View logs of a container.                                                                     | `docker logs <container_id>`                                               |
| `docker inspect`    | Get detailed information about a container.                                                   | `docker inspect <container_id>`                                            |
| `docker stats`      | Display live resource usage statistics for containers.                                        | `docker stats`                                                             |
| `docker attach`     | Attach to a running container's terminal.                                                     | `docker attach <container_id>`                                             |

---

## **3. Image Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker images`     | List locally stored images.                                                                   | `docker images`                                                            |
| `docker pull`       | Pull an image from a registry (e.g., Docker Hub).                                             | `docker pull nginx`                                                        |
| `docker push`       | Push an image to a registry.                                                                  | `docker push myrepo/myimage:tag`                                           |
| `docker build`      | Build an image from a Dockerfile.                                                             | `docker build -t myimage:tag .`                                            |
| `docker rmi`        | Remove one or more images.                                                                    | `docker rmi <image_id>`                                                    |
| `docker tag`        | Tag an image for a repository.                                                                | `docker tag <image_id> myrepo/myimage:tag`                                 |
| `docker history`    | Show the history of an image.                                                                 | `docker history <image_id>`                                                |
| `docker save`       | Save an image to a tar archive.                                                               | `docker save -o myimage.tar myimage:tag`                                   |
| `docker load`       | Load an image from a tar archive.                                                             | `docker load -i myimage.tar`                                               |

---

## **4. Network Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker network ls` | List networks.                                                                                | `docker network ls`                                                        |
| `docker network create` | Create a new network.                                                                     | `docker network create mynetwork`                                          |
| `docker network inspect` | Inspect a network.                                                                        | `docker network inspect bridge`                                           |
| `docker network rm` | Remove a network.                                                                             | `docker network rm mynetwork`                                              |
| `docker network connect` | Connect a container to a network.                                                         | `docker network connect mynetwork <container_id>`                          |
| `docker network disconnect` | Disconnect a container from a network.                                                 | `docker network disconnect mynetwork <container_id>`                       |

---

## **5. Volume Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker volume ls`  | List volumes.                                                                                 | `docker volume ls`                                                         |
| `docker volume create` | Create a new volume.                                                                       | `docker volume create myvolume`                                            |
| `docker volume inspect` | Inspect a volume.                                                                         | `docker volume inspect myvolume`                                           |
| `docker volume rm`  | Remove a volume.                                                                              | `docker volume rm myvolume`                                                |
| `docker volume prune` | Remove unused volumes.                                                                      | `docker volume prune`                                                      |

---

## **6. Docker Compose Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker-compose up` | Start and attach to containers defined in a `docker-compose.yml` file.                        | `docker-compose up -d`                                                     |
| `docker-compose down` | Stop and remove containers, networks, and volumes defined in a `docker-compose.yml` file.   | `docker-compose down`                                                      |
| `docker-compose ps` | List containers managed by Docker Compose.                                                    | `docker-compose ps`                                                        |
| `docker-compose logs` | View logs of services defined in a `docker-compose.yml` file.                               | `docker-compose logs`                                                      |
| `docker-compose build` | Build or rebuild services.                                                                | `docker-compose build`                                                     |
| `docker-compose restart` | Restart services.                                                                        | `docker-compose restart`                                                   |
| `docker-compose scale` | Scale services.                                                                          | `docker-compose scale service_name=3`                                      |

---

## **7. Miscellaneous Commands**
| **Command**         | **Purpose**                                                                                   | **Example**                                                                 |
|---------------------|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| `docker version`    | Show Docker version information.                                                              | `docker version`                                                           |
| `docker info`       | Display system-wide information (e.g., number of containers, images, etc.).                   | `docker info`                                                              |
| `docker login`      | Log in to a Docker registry.                                                                  | `docker login`                                                             |
| `docker logout`     | Log out from a Docker registry.                                                               | `docker logout`                                                            |
| `docker search`     | Search for images on Docker Hub.                                                              | `docker search nginx`                                                      |
| `docker cp`         | Copy files/folders between a container and the local filesystem.                              | `docker cp <container_id>:/path/to/file /local/path`                       |

---

## **Key Notes**
1. Replace placeholders like `<container_id>`, `<image_id>`, and `<network_name>` with actual values.
2. Use `-d` for detached mode when running containers.
3. Use `-it` for interactive terminal access when using `docker exec`.
4. Use `--help` after any command for additional options. Example: `docker run --help`.