# Jenkins Configuration

This is a jenkins configuration to run on a docker-enabled server.

## Local Development Setup

1. Clone the repository.
2. Run the docker with docker-compose `docker-compose up -d`.
3. Ensure your hosts setup directs jenkins.localhost to 127.0.0.1.
4. Navigate to http://jenkins.localhost in your browser and go through Jenkins set up.

## Production Setup

1. Clone the repository.
2. Copy .env-dist to .env and fill in the JENKINS_URL with the public url for the new jenkins.
3. Run the docker with docker-compose `docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d`.
4. Navigate to to the url you specified in step 2 in your browser and go through Jenkins set up.