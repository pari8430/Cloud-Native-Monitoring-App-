# Cloud Native Monitoring App

A cloud-native application designed to monitor and manage AWS resources using Kubernetes, Docker, and Flask. The app provides real-time monitoring of AWS services, enabling easy access to metrics and health statuses.

## Description

The Cloud Native Monitoring App is built to help users monitor their cloud infrastructure, specifically AWS resources, such as ECR and EKS. The app is containerized using Docker and orchestrated using Kubernetes for scalability and management. It features a user-friendly interface built with Flask to display monitoring metrics and logs.

## Features

- **Real-time monitoring** of AWS services (ECR, EKS, etc.)
- Scalable microservices architecture using **Kubernetes** and **Docker**
- **Flask**-based web interface for interacting with the monitoring system
- Easily deployable on any cloud-native platform
- **AWS SDK (Boto3)** integration for fetching real-time metrics
- Dockerized for isolated environment setup
- Kubernetes deployments for high availability

## Technologies Used

- **AWS**: Amazon Elastic Container Registry (ECR), Amazon Elastic Kubernetes Service (EKS)
- **Kubernetes**: For container orchestration and microservice deployment
- **Docker**: Containerization for isolated development and deployment environments
- **Flask**: Web framework for the user interface and application logic
- **Python**: Main programming language
- **Boto3**: AWS SDK for Python to interact with AWS resources
- **Helm**: Kubernetes package manager for easier management of Kubernetes charts

## Prerequisites

Before you begin, ensure that you have the following installed on your system:

- **Python 3.6+**: Install Python from [python.org](https://www.python.org/downloads/)
- **Docker**: Install Docker from [docker.com](https://www.docker.com/products/docker-desktop)
- **Kubernetes**: Install Kubernetes and set up a cluster (local or cloud)
- **AWS CLI**: Install the AWS CLI and configure your AWS credentials (`aws configure`)
- **kubectl**: Kubernetes CLI for interacting with your Kubernetes cluster

## Installation

Follow these steps to set up the project on your local machine.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/cloud-native-monitoring-app.git
   cd cloud-native-monitoring-app


2. **Set up a virtual environment:**

The application uses the **`psutil`** and **`Flask`, Plotly, boto3** libraries. Install them using pip:
```
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

```

3. **Run the application**

Install the required dependencies:

```
pip install -r requirements.txt

```
4. **Configure your AWS credentials (e.g., using aws configure):**
    ```aws configure
    ```

5. **Run the application:**
   ```
python app.py

```   
6. Access the app through your local server (e.g., http://localhost:5000).

#### f. **Usage**
Explain how to use the application. Provide examples if applicable, such as how to interact with the app or access different features.

```markdown
## Usage

Once the app is running, navigate to `http://localhost:5000` in your browser to view the monitoring dashboard. The dashboard will show real-time metrics of your AWS resources.

Example commands to run the app with Docker:

```bash
docker build -t monitoring-app .
docker run -p 5000:5000 monitoring-app


#### g. **Screenshots/Visuals**

```markdown
## Screenshots

![Dashboard Screenshot](screenshot.png)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thank you to the developers of Flask, Docker, and Kubernetes for their excellent frameworks and tools.


