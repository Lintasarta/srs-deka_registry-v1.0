# Software Interface

The Deka Container Registry product will be accessible via the company's service portal on cmd.cloudeka.id and ai.cloudeka.id, which will act as the frontend. The backend services supporting the registry will manage image storage, authentication, and distribution.

- **Platform: Kubernetes (Version: 1.24+)**  
  The backend services of the Deka Container Registry are assumed to be deployed on Kubernetes. This ensures efficient orchestration, scalability, and high availability of the container registry services and associated microservices. Kubernetes manages the deployment, scaling, and lifecycle of these backend components.

- **Backend: Harbor (Open-Source Container Registry)**  
  The core of the Deka Container Registry is assumed to leverage Harbor, a leading open-source cloud-native registry project. Harbor extends the capabilities of the Docker Distribution with enterprise-grade features. This backend will be responsible for:
  - Storing and managing container images and OCI artifacts.
  - Handling image push, pull, and delete operations.
  - Managing repository metadata and project-level configurations.
  - Implementing authentication and authorization logic, integrating with Deka's identity management systems.

- **Database: PostgreSQL (Version: 14+)**  
  The backend stores registry metadata, user data, access logs, image manifests, and configuration settings in a PostgreSQL database. This provides a robust, scalable, and reliable data storage solution for the registry's operational data.
