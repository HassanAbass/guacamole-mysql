# Guacamole Docker Compose Setup

This Docker Compose configuration allows you to quickly set up a Guacamole server with PostgreSQL as the backend database and Guacd as the Guacamole proxy. Guacamole is an open-source remote desktop gateway that provides access to your systems over various protocols.

## Prerequisites

Before using this Docker Compose setup, ensure that you have Docker and Docker Compose installed on your system.

- [Docker Installation Guide](https://docs.docker.com/get-docker/)
- [Docker Compose Installation Guide](https://docs.docker.com/compose/install/)

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone git@github.com:HassanAbass/guacamole-mysql.git
2. Create psql dir to persist data

   ```bash
   mkdir postgres_data
3. Start docker compose

   ```bash
   docker-compose up -d
4. Access Guacamole by navigating to http://localhost:8080/guacamole in your web browser. 
    >
        The default credentials are:
        Username: guacadmin
        Password: guacadmin

## Important Notes:

The PostgreSQL data and schema directories are mounted as volumes. Ensure the permissions are set appropriately for these directories.
Guacamole's web interface is accessible at http://localhost:8080/guacamole. Adjust the port as needed.