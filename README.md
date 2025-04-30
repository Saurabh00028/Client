# Client
Demo Project
---

## 📦 Microservices Components

### 🔧 Config Server
- Centralized external configuration management.
- Enables dynamic updates to service configuration without redeployment.

### 📘 Eureka Server
- Service discovery mechanism.
- All microservices register themselves to enable load balancing and fault tolerance.

### 📦 Order Service
- Handles customer orders.
- Communicates with the orchestrator service using Feign clients.

### 📦 Orchestrator Service
- Coordinates communication between Order, Payment, and Inventory services.
- Contains core business logic for order processing.

### 💳 Payment Service
- Processes and verifies payments.
- Communicates with Orchestrator.

### 📦 Inventory Service
- Manages stock levels and inventory data.
- Validates product availability during orders.

### 📩 Notification Service
- Sends emails or push notifications for order events.

---

## 📡 Communication

- **Service Discovery:** All services register with Eureka Server.
- **Inter-Service Communication:** Uses Feign clients for declarative REST calls.
- **Configuration:** Pulled dynamically from the Config Server.

---


## 🚀 How to Run

1. **Start Config Server**
2. **Start Eureka Server**
3. **Start individual microservices (Order, Orchestrator, etc.)**
4. Ensure all services register in Eureka dashboard.

---

---

## 📬 Contact

For issues or enhancements, please open an issue or contact the maintainer.

---

