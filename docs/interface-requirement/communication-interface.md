# Communication Interface

- **Frontend (Service Portal) to Backend**  
  The service portal (cmd.cloudeka.id and ai.cloudeka.id) communicates with the Deka Container Registry backend services using HTTPS REST API calls. This ensures secure transmission of data and commands between the user interface and the registry's core functionalities. The communication may also include authentication tokens or session identifiers for secure user interactions.

- **Docker CLI / Client Tools to Backend**  
  Standard Docker CLI commands (docker push, docker pull, docker login) and other OCI-compliant client tools communicate directly with the Deka Container Registry backend using the Docker Registry HTTP API V2 protocol over HTTPS. This secure connection facilitates the efficient transfer of container images and metadata.

- **Backend to Database (PostgreSQL)**  
  The backend interacts with the PostgreSQL database over a secure connection using the standard PostgreSQL protocol. This allows the backend to store and retrieve data related to image manifests, user permissions, repository configurations, usage metrics, and other application-specific information.
