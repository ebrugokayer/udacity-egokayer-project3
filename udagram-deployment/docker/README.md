## Setup Instructions

### Environment Variables

Set environment variables for config values such as the database connection. The required environment values can be found in the docker-compose.yaml file.

### Setup Docker Environment

You'll need to install docker https://docs.docker.com/install/. Open a new terminal within the project directory and run:

1. Build the images: docker-compose -f docker-compose-build.yaml build --parallel
2. Push the images: docker-compose -f docker-compose-build.yaml push
3. Run the container: docker-compose up