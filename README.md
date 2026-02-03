# Bank Account Config Repo - Centralized Configuration for Microservices

This repository serves as the **central configuration server repository** for a microservices-based banking application using **Spring Cloud Config**.  
It stores externalized configuration properties for multiple services (e.g., account-service and customer-service) across different environments (default, dev, prod).

Configurations are version-controlled here and can be pulled dynamically by client services via Spring Cloud Config Server.

## Purpose
- Centralize all configuration in one place (Git-backed).
- Support environment-specific profiles (dev, test, prod).
- Enable easy updates without redeploying services.
- Ideal for microservices architecture in banking/fintech apps (account management, customer data...).

## Tech Stack
- **Configuration Format**: Spring Boot Properties files (.properties)
- **Backend**: Designed for Spring Cloud Config Server (Java/Spring Boot ecosystem)
- **Version Control**: Git (this repo)
- **Environments Supported**: default, dev, prod

## Repository Structure
bank-account-config-repo/
├── account-service.properties          # Default config for account-service
├── account-service-dev.properties      # Dev profile overrides
├── account-service-prod.properties     # Prod profile overrides
├── customer-service.properties         # Default config for customer-service
├── customer-service-dev.properties     # Dev profile overrides
├── customer-service-prod.properties    # Prod profile overrides
├── application.properties              # Optional global/default config
└── README.md
