# Fortune Tracker Server

## About This Project
This is a backend api service integrated with MariaDB and MongoDB for an application that manages your daily ledgers. Users can hold personal and shared ledgers to record their daily transactions more conveniently.

## Usage
You can view the API document here : []

## Run Fortune-Tracker API Yourself
First clone this repository: 
```
git clone https://github.com/yu-niverse/Fortune-Tracker.git
cd Fortune-Tracker
```
Follow the following steps to run the service :

### Prerequisites
1. Install Docker and Docker Compose
    <br/>( you can run the following script to install the same version )
   
    ```
    chmod +x fortune-tracker-docker/install.sh
    ./fortune-tracker-docker/install.sh
    ```
2. Configure your own `app.env`
   
### Run the Service
```
cd fortune-tracker-docker
docker compose --env-file app.env up -d
```
You can view the status of the containers by running

```
docker compose --env-file app.env ps
```

The log files will be under `logs` directory or view the logs manually by running

```
docker compose --env-file app.env logs <service_name>
```
