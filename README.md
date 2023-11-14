# Job Portal

![Job Portal Logo/Icon]

## Overview

Welcome to the Job Portal project! This application is designed to serve as a comprehensive job board where employers can post job vacancies, and job seekers can discover, search, and apply for available positions. The project utilizes the Tall Stack - TailwindCSS, AlpineJS, Livewire, and Laravel - to create a modern, responsive, and efficient platform.

### Features

- **Employer Dashboard:** Enables employers to post job vacancies, manage listings, and review applicant submissions.
- **Job Seeker Interface:** Provides a user-friendly interface for job seekers to search, view, and apply for job openings.
- **Resume Parsing:** Includes functionality to parse and extract relevant information from resumes uploaded by job seekers.
- **Notifications:** Incorporates a notification system to keep users updated on application statuses, new job postings, etc.

### Technology Stack

- **Frontend:** TailwindCSS, AlpineJS, Livewire
- **Backend:** Laravel
- **Containerization:** Docker
- **Scaling & Orchestration:** Kubernetes

### Prerequisites

- PHP 8.1 or higher
- MySQL 8.0 or higher
- Laravel 10 or higher
- Livewire 3.x or higher
- AlpineJS 3.x.x or higher
- TailwindCSS 3.x or higher
- Install Docker on your machine: [Docker Installation Guide](https://docs.docker.com/get-docker/)
- Set up Kubernetes for orchestration: [Kubernetes Setup Guide](https://kubernetes.io/docs/setup/)

### Getting Started

To run this project locally, follow these steps:
1. Clone this repository: [Job Board GitHUb Repo](https://github.com/farhanali-developer/job-board.git)
2. Install the dependencies:
 - cd job-portal
 - composer install
 - npm install
3. Create a database and configure the application:
 - cp .env.example .env
 - php artisan key:generate
 - php artisan migrate
4. Start the development environment:
 - docker-compose up -d
5. Access the application in your browser at http://localhost:8080

### Database Setup

1. Run database migrations and seeders if needed:
 - docker-compose exec app php artisan migrate --seed

### Testing

1. Implement and execute tests for various functionalities using PHPUnit or other testing frameworks:
 - docker-compose exec app ./vendor/bin/phpunit

### Deployment

To deploy the application to Kubernetes, follow these steps:
1. Build the Docker image:
 - docker build -t farhanali/job-portal:latest
2. Push the Docker image to a registry:
 - docker push farhanali/job-portal:latest
3. Create a Kubernetes deployment file:
 - kubectl apply -f deployment.yaml
4. Create a Kubernetes service file:
 - kubectl apply -f service.yaml
5. Access the application in your browser at the service's external IP address

### Contributing

Contributions are welcome! To contribute, please create a pull request with your changes.

### Author

Farhan Ali (https://github.com/farhanali-developer)

### Contributing

Contributions to enhance features, fix bugs, or optimize performance are welcome! Please fork the repository, make your changes, and submit a pull request.