# Cloud Native Monitoring App

This is a cloud-native monitoring app designed to monitor AWS resources and provide real-time metrics via a web dashboard. The app is built using Flask and containerized using Docker. It is deployed using Kubernetes for scalability and easy management.

## Table of Contents
- [Project Setup](#project-setup)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [License](#license)
- [Acknowledgments](#acknowledgments)


## Features

- Real-time monitoring of AWS services (ECR, EKS, etc.)
- Scalable with Kubernetes for cloud-native deployment
- Containerized microservices using Docker
- User-friendly UI built with Flask

## Technologies Used

- **AWS**: ECR, EKS
- **Kubernetes**: Deployment and orchestration of containerized apps
- **Docker**: Containerization
- **Flask**: Web framework for the user interface
- **Python**: Core programming language
- **Boto3**: AWS SDK for Python

## Project Setup

### Prerequisites

- Docker
- Python 3.x
- Kubernetes Cluster (if deploying on Kubernetes)
- AWS CLI configured with your AWS credentials
- Access to ECR (Elastic Container Registry) to pull the Docker image

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/cloud-native-monitoring-app.git
    cd cloud-native-monitoring-app
    ```

2. Install the required Python dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. If deploying with Kubernetes, ensure you have the correct kubeconfig file set up for your cluster.

## Running the Application

### a. **Docker Setup**

To run the app locally with Docker:

1. Build the Docker image:

    ```bash
    docker build -t monitoring-app .
    ```

2. Run the Docker container:

    ```bash
    docker run -p 5000:5000 monitoring-app
    ```

This will start the Flask application on `http://localhost:5000`.

### b. **Kubernetes Deployment**

If deploying the app on Kubernetes, create the necessary deployments and services. Follow these steps:

1. Create a Kubernetes deployment file (e.g., `deployment.yaml`) for the app.
2. Apply the deployment:

    ```bash
    kubectl apply -f deployment.yaml
    ```

### c. **Access the App**

Once the app is running, navigate to `http://localhost:5000` in your browser to view the monitoring dashboard. The dashboard will show real-time metrics of your AWS resources.

## Usage

Once the app is running, navigate to `http://localhost:5000` in your browser to view the monitoring dashboard. The dashboard will display real-time metrics such as CPU, memory usage, and other vital AWS resource information.

Example commands to run the app with Docker:

```bash
docker build -t monitoring-app .
docker run -p 5000:5000 monitoring-app
```

## Screenshots

Below are some screenshots of the Cloud Native Monitoring App's dashboard:

![Dashboard Screenshot](images/newplot.png)
![Dashboard Screenshot](images/newplotnew.png)
*Example of the monitoring dashboard showing AWS resource metrics.*

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thank you to the developers of Flask, Docker, and Kubernetes for their excellent frameworks and tools.




