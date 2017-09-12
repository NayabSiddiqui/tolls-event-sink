# Tolls Spring Cloud Event-Sink

Spring boot based app to act as a events-sink for spring cloud task.
It listens on events in the [RabbitMQ](https://www.rabbitmq.com/) queue messages and kicks of the task.


### How to set up Dev Environment

  #### Prerequisites:
- Docker. To install docker on your machine, go [here](https://www.docker.com/)
- Gradle

#### Get Started:

- Start a RabbitMQ instance with the management plugin:

    Get the Docker container running by issuing the following command:
    ```
    docker run -d --hostname spring-cloud-rabbit --name spring-cloud-rabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management
    ```
    
    This starts up the RabbitMQ instance listening on the host at port `5672`. 
    The management plugin for the same can be accessed at `http://localhost:15672`.
    
- Run the application:

    Run the application by issuing following command on command line:
    ```
    gradle bootRun
    ```
    
---

    