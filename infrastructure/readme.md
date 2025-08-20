## **Infrastructure**

This section details the infrastructure I implemented to containerize and manage the project's environment for consistent and reproducible deployments.


### Containerization and Environment Setup

I used **Docker** to containerize the application's different services, ensuring the entire environment is portable and reproducible. The project setup includes a `Makefile` to streamline common development and deployment tasks, such as building Docker images and starting services. This approach guarantees that dependencies are managed consistently across development, staging, and production environments.
