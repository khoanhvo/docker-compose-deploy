# InfluxDB 2.0 Docker Compose

This Docker Compose file allows you to easily set up and run InfluxDB 2.0 using Docker.

## Prerequisites

- Docker installed on your machine

## Usage

1. Clone this repository to your local machine.

2. Navigate to the `docker-compose-src/influxdb2` directory.

3. Open a terminal and run the following command to start the InfluxDB container:

   ```bash
   docker-compose up -d
   ```

4. InfluxDB will be accessible at `http://localhost:8086`.

## Configuration

The `docker-compose.yml` file contains the following configuration options:

- `image`: Specifies the InfluxDB 2.0 Docker image to use.

- `ports`: Maps the container's port 8086 to the host's port 8086, allowing access to InfluxDB.

- `volumes`: Mounts the `influxdb-data` directory on the host machine to the `/var/lib/influxdb2` directory inside the container, allowing data persistence.

- `environment`: Sets up the initial configuration for InfluxDB. Modify the values of the environment variables to suit your needs.

## Cleanup

To stop and remove the InfluxDB container, run the following command:
`bash
    docker-compose down
    `
