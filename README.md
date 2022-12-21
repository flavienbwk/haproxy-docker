# HAProxy Docker

Example of HAProxy implementation with Docker. Serving web servers.

HAProxy allows performing load-balancing actions to avoid SPF (single points of failure).

## Start

1. Run the containers

    ```bash
    docker-compose up -d
    ```

2. Access HAProxy : [`http://localhost:8080`](http://localhost:8080)

    Access the HAProxy panel at [`http://localhost:8404`](http://localhost:8404)

    To update HAProxy configuration [without service interuption](https://serverfault.com/questions/1026631/how-to-send-a-signal-to-a-docker-container-without-affecting-restart-policy), run the following command :

    ```bash
    docker kill -s HUP haproxy
    ```
