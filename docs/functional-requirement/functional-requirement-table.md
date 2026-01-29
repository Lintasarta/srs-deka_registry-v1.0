# Functional Requirement Table

| ID      | Functional Requirement   | Description |
|---------|--------------------------|-------------|
| REG-001 | Registry Creation        | Users (Useradmin/Superadmin) can create new container registries (projects in Harbor terminology) within their organizations via Cloudeka Service Portal. |
| REG-002 | Registry Management      | Users (Useradmin/Superadmin) can view, edit (e.g., change name, description, access level, resize), and delete existing container registries via Cloudeka Service Portal. |
| REG-003 | Image Push               | Authenticated users can push Docker images and OCI artifacts to designated repositories within a registry using Docker CLI or other compatible tools. |
| REG-004 | Image Pull               | Authenticated users can pull Docker images and OCI artifacts from designated repositories within a registry using Docker CLI or other compatible tools. |
| REG-005 | Image Tagging            | Users can tag images with multiple versions, allowing for proper version control and release management. |
| REG-006 | Image Deletion           | Authenticated users with appropriate permissions can delete specific images or image tags from repositories. |
| REG-007 | Repository Management    | Users can create, view, and delete repositories within a registry via Cloudeka Service Portal or CLI. |
| REG-008 | User Authentication      | The registry must support authentication for users and service principals to securely access registry operations (e.g., docker login). This includes integration with Deka's central authentication system. |
| REG-009 | RBAC                     | Users (Useradmin/Superadmin) can add members to the registry (projects in Harbor terminology) within their organizations via Cloudeka Service Portal. |
| REG-010 | Audit and Activity Logs  | Users (Useradmin/Superadmin) can view detailed audit and activity logs for all operations performed on the registry (e.g., image pushes, pulls, deletions, access attempts, policy changes). |
