# OrderFoodDeliveryMicroservices

## Overview
OrderFoodDeliveryMicroservices is a project demonstrating a microservices-based architecture for a food ordering and delivery system. The project includes multiple microservices, each responsible for a specific functionality within the system. This implementation uses Spring Boot and integrates Eureka for service discovery.

## Microservices
The system consists of the following microservices:

1. **Order Service**
   - Manages customer orders.
   - Provides APIs to create, view, and update orders.

2. **Customer Management Service**
   - Handles customer information.
   - Provides APIs for customer registration and management.

3. **Payment Service**
   - Manages payment processing.
   - Provides APIs for payment-related actions.

4. **Restaurant Service**
   - Handles restaurant and menu information.
   - Provides APIs to manage restaurant data and menus.

## Architecture
- **Service Discovery**: Eureka is used for dynamic service registration and discovery.
- **Inter-Service Communication**: REST APIs are used for communication between microservices.
- **Database**: Each microservice uses its own database for data persistence.

## Demonstration
You can find the demonstartion video in the main directory 

## Prerequisites
Before running the project, ensure you have the following installed:
- Java 11 or later
- Maven
- Git
- Docker (optional, for containerized deployment)

## Getting Started

### Clone the Repository
```bash
git clone https://github.com/ABDULMAJEED7778/OrderFoodDeliveryMicroservices.git
cd OrderFoodDeliveryMicroservices
```

### Build and Run the Project
1. **Build the project**:
   ```bash
   mvn clean install
   ```

2. **Run the Eureka Server**:
   Navigate to the Eureka Server directory and run:
   ```bash
   mvn spring-boot:run
   ```

3. **Run the microservices**:
   Navigate to each microservice directory and run:
   ```bash
   mvn spring-boot:run
   ```

### Access the Services
- **Eureka Dashboard**: [http://localhost:8761]
- **Order Service**: [http://localhost:9001]
- **Customer Management Service**: [http://localhost:9002]
- **Payment Service**: [http://localhost:9003]
- **Restaurant Service**: [http://localhost:9004]

## Sample Data
- Sample JSON files for each entity (Customer, Order, Payment, Restaurant, etc.) are included in the `data` folder for testing purposes.

## Key Features
- **Modular Design**: Each microservice handles a specific domain.
- **Service Discovery**: Dynamic registration and discovery using Eureka.
- **Scalability**: Independent scalability of microservices.

## Future Enhancements
- Integration with RabbitMQ for asynchronous communication.
- Adding a Gateway service for centralized routing.
- Implementing OAuth2 for secure API access.



---
