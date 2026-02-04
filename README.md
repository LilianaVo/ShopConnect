<div align="center">

# ShopConnect: Distributed E-Commerce Platform

### A scalable, containerized e-commerce solution built with a microservices architecture.

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)

[View Demo] • [Report Bug] • [Request Feature]

</div>

---

## Overview

**ShopConnect** is a robust simulation of a distributed e-commerce system designed to handle concurrent user transactions and ensure data consistency.

Unlike a monolithic application, this platform utilizes **Docker containers** to isolate services (Frontend, Backend, and Database), simulating a real-world production environment where scalability and fault tolerance are critical.

**Key Engineering Concepts Applied:**
* **Microservices Architecture:** Decoupled components for independent deployment.
* **Containerization:** Full orchestration using `docker-compose`.
* **Concurrency Control:** Handling multiple simultaneous purchase requests without data race conditions.
* **Persistence:** Docker volumes for reliable data storage.

---

## Academic Context

This project was developed as the **Final Capstone** for the **Distributed Systems** course at the **National Autonomous University of Mexico (UNAM)**.

| **Course Information** | **Details** |
| :--- | :--- |
| **University** | Universidad Nacional Autónoma de México (UNAM) |
| **Faculty** | **Facultad de Ingeniería (FI)** |
| **Course** | Sistemas Distribuidos (Distributed Systems) |
| **Professor** | M.I. Jasmine Macedo Reza |
| **Semester** | 2026-1 |
| **Group** | 01 |

---

## System Architecture

The system follows a client-server model orchestrated via Docker:

1.  **Frontend Service:** Interactive UI built with React for product catalog and shopping cart management.
2.  **Backend Service:** Flask API handling business logic, transaction processing, and inventory updates.
3.  **Database Service:** MySQL relational database ensuring ACID compliance for transactions.
4.  **Adminer:** Database management tool integrated for real-time monitoring.

---

## Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Infrastructure** | **Docker & Docker Compose** | Container orchestration and environment setup. |
| **Backend** | **Python (Flask)** | RESTful API development and logic. |
| **Frontend** | **React / HTML5 / CSS3** | Responsive user interface. |
| **Database** | **MySQL** | Persistent data storage. |
| **Management** | **Adminer** | Database administration interface. |

---

## Getting Started

To run **ShopConnect** locally, you only need Docker installed. No other dependencies are required on your host machine.

### Prerequisites
* Docker Engine
* Docker Compose

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/LilianaVo/ShopConnect.git](https://github.com/LilianaVo/ShopConnect.git)
    ```

2.  **Navigate to project directory**
    ```bash
    cd ShopConnect
    ```

3.  **Build and Run Services**
    ```bash
    docker-compose up --build
    ```

4.  **Access the Application**
    Open your browser and navigate to: `http://localhost:5000` (or your specific port).

---

## Contributors & Development Team

This project was a collaborative effort by the following engineering students:

* **Ileana Verónica Lee Obando** - *DevOps & Container Orchestration*
* **Luis Enrique Cruz Hernández**
* **Deissy Jovita Hernández Hernández**
* **Javier Antonio Rodríguez García**
* **Carlos Andrés Troncoso González**
* **Wendy Jazmin Trujillo Salazar**

**My Contributions (Ileana Lee):**
* **DevOps & Infrastructure:** Engineered the `Dockerfile` and `docker-compose.yml` to ensure seamless deployment across different environments.
* **Frontend Development:** Designed the user interface and integrated the client-side logic with the REST API.
* **Database Integration:** Managed the connection strings and environment variables for secure container linking.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
