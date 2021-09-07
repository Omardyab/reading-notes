#  Reading 25: Docker

- Entire development environment is isolated.
- Can be shared among team members.
- Complexity is a downside.
- Docker is really just Linux containers.
- The downside to a virtual machine:Size and speed.
- Using Linux: provide a lightweight, faster way to duplicate much of the same functionality
- “Containerization,” has become increasingly popular. For most applications, a virtual machine provides far more resources than are needed and a container is more than sufficient.
- Docker is. A way to implement Linux containers!
- Containers are like apartments: they share common infrastructure like plumbing and heating, but come in various sizes that match the exact needs of an owner.
- Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great. But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

- after downloading Docker, :

        docker --version, confirm the correct version is running
        docker run hello-world //confirm Docker installed correctly 
        docker info //inspect Docker

## Images and Containers

- An image is a snapshot in time of what a project contains.
- A container is a running instance of the image.
- A baking analogy we can use here is as follows:

        A Dockerfile is the recipe for a cake
        An image is a snapshot of the recipe at a given time
        A docker-compose.yml says how to make the cake
        And the container is the actual, baked cake

## Image Layers

- This is called image layering and it exists for two main reasons. First, each image layer is immutable–unchanged–like a git commit.
- This is called image layering and it exists for two main reasons. First, each image layer is immutable–unchanged–like a git commit.

## Dockerized Django

Order matters in Dockerfiles since they are executed from top-to-bottom.

### The important takeaways from this tutorial are this

        Docker is a way to run Linux containers
        Containers are a lightweight alternative to Virtual Machines
        Dockerfile is a list of instructions for creating an image
        Images are made up of one or more layers
        Containers are a running instance of an image
        docker-compose.yml controls how to run the container
        Containers are stateless and ephemeral in nature. 
        We can link the local filesystem via volumes but things become more complex with databases.
