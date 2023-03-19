Build a Docker:
`docker build -t app:docker_nodejs .`

List containers:
`docker ps`

Run the Docker image. Add name, port forwarding, CPU and memory usage:
`docker run --name docker_nodejs -p 80:80 --cpus=4 --memory=1024m app:docker_nodejs`

Run the Docker image from the Docker Hub. Add name, port forwarding, CPU and memory usage:
`docker run --name docker_nodejs -p 80:80 --cpus=4 --memory=1024m <username>/docker_nodejs:v1.0`

Sign in to the Docker Hub
`docker login`

Add a Docker tag:
`docker tag <docker_image_id> <username>/docker_nodejs:v1.0`

Push a image to the Docker Hub:
`docker push <username>/docker_nodejs:v1.0`

Pull the Docker image
`docker pull <username>/docker_nodejs:v1.0`

List of pulled images
`docker images`
