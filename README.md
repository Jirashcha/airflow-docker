# Airflow-Docker

Practicing Apache Airflow using Docker.

## Prerequisites

- Docker installed  
  👉 [Download Docker](https://www.docker.com/products/docker-desktop)

## Setup Steps

1. **Install Docker**  
   Follow the instructions from the Docker website.

2. **Download the Airflow Docker Compose file**  
   Visit: [Airflow Docker Setup Guide](https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html)

3. **Download the `docker-compose.yaml` file**  
   Open this URL in your browser and save the file:  
   [https://airflow.apache.org/docs/apache-airflow/2.11.0/docker-compose.yaml](https://airflow.apache.org/docs/apache-airflow/2.11.0/docker-compose.yaml)

4. **Open Terminal and run the following:**

   ```bash
   mkdir airflow-docker
   cd airflow-docker
   move ~/Downloads/docker-compose.yaml .
   code .
   ```
5. **Customize your setup (optional)**
   - Edit configuration files if needed.

6. **Start Airflow using Docker Compose:**
  ```bash
  docker-compose up
  ```
7. Open a new terminal and initialize the Airflow database:
  ```bash
  docker-compose exec airflow-scheduler bash
  ```
  ```bash
  airflow db init
  ```
9. Create an Airflow user:
  ```bash
  airflow users create
  ```
  - Fill in the required information such as username, password, email, role, and first/last name.

## ✅ After setup, access the Airflow web UI at:
http://localhost:8080

![image](https://github.com/user-attachments/assets/5ba89d6b-3358-456b-bc15-0b98d4977e48)
