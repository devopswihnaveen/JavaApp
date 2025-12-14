# JavaApp

## Overview
This repository contains the Java application source code. For infrastructure-as-code deployment on AWS, refer to the separate [terraform-aws-infrastructure](https://github.com/your-org/terraform-aws-infrastructure) repository.

## Prerequisites
- Java 11 or higher
- Maven 3.6+ (or Gradle 6.0+)
- Git

## Project Structure
```
JavaApp/
├── src/
│   ├── main/
│   │   ├── java/        # Application source code
│   │   └── resources/   # Configuration files
│   └── test/            # Unit tests
├── pom.xml              # Maven configuration
├── Dockerfile           # Container image definition
└── README.md            # This file
```

## Building

### Compile
```bash
mvn clean compile
```

### Run Tests
```bash
mvn test
```

### Build JAR
```bash
mvn clean package
```

### Build Docker Image
```bash
docker build -t javaapp:latest .
```

## Running Locally
```bash
java -jar target/javaapp.jar
```

## Deployment
For AWS infrastructure deployment, see the [terraform-aws-infrastructure](https://github.com/devopswihnaveen/terraform-aws-infrastructure) repository and [EKS configuration](https://github.com/devopswihnaveen/aws-eks-ci-cd) repository.

## Support
For issues, create a GitHub issue or refer to project documentation.