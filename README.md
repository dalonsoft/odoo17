# odoo17
Odoo 17 enviroment in docker containers

### Creating a .env File

To create a `.env` file from the example file, follow these steps:

1. Copy the example file:
    ```sh
    cp .env.example .env
    ```

2. Open the `.env` file in a text editor and configure the parameters as needed.

#### Parameters Description

- `NGINX_EXPOSED_PORT`: The port on which the Nginx server will be exposed.
- `NGINX_SSL_CERTIFICATE_PATH`: The path to the SSL certificate file.
- `NGINX_SSL_CERTIFICATE_KEY_PATH`: The path to the SSL certificate key file.
- `POSTGRES_DB`: The name of the PostgreSQL database
- `POSTGRES_USER`: The username for the PostgreSQL database
- `POSTGRES_PASSWORD`: The password for the PostgreSQL database

Make sure to replace the placeholder values with the actual configuration for your environment.

Remember to keep the `.env` file private and never commit it to a public repository.

In Plesk, you can find the SSL certificate and key files in the following directory:

/usr/local/psa/var/modules/sslit/etc/live/your_domain/cert.pem
/usr/local/psa/var/modules/sslit/etc/live/your_domain/privkey.pem

```

### Starting the Odoo 17 Docker Environment

To start the Odoo 17 Docker environment, run the following command:

```sh
docker-compose up -d
```

This command will start the Odoo 17 server, PostgreSQL database, and Nginx server in the background.

### Stopping the Odoo 17 Docker Environment

To stop the Odoo 17 Docker environment, run the following command:

```sh
docker-compose down
```

This command will stop and remove the Odoo 17 server, PostgreSQL database, and Nginx server containers.