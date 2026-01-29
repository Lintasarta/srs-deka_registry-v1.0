# Use Case Description

**Action and Response**

| Action by user | Response from system |
|---------------|----------------------|
| Useradmin/Superadmin initiates creation of a new registry (project) via Service Portal. | System displays registry creation form, then creates the registry (project) in Harbor. |
| Useradmin/Superadmin views the list of existing registries. | System displays a list of all accessible registries with their key details. |
| Useradmin/Superadmin edits properties of an existing registry. | System updates the registry's configuration (e.g., name, description, access level). |
| Useradmin/Superadmin confirms deletion of a registry. | System deletes the specified registry and all its associated contents (repositories, images, metadata). |
| Authenticated user executes docker push &lt;registry-url&gt;/&lt;repo&gt;/&lt;image&gt;:&lt;tag&gt;. | System receives image layers and manifest, stores them, and initiates vulnerability scan. |
| Authenticated user executes docker pull &lt;registry-url&gt;/&lt;repo&gt;/&lt;image&gt;:&lt;tag&gt;. | System retrieves image layers and manifest, and transfers them to the client. |
| User tags an image (e.g., via Docker CLI docker tag or Service Portal). | System associates the new tag with the image's manifest within the repository. |
| Authenticated user deletes a specific image tag or an entire image via CLI or Service Portal. | System removes the image tag and associated data (if no other tags reference the image layers). |
| User creates a new repository within a registry via Service Portal or CLI. | System creates the new repository. |
| User views the contents of a specific repository via Service Portal or CLI. | System displays a list of all images and their tags within the specified repository. |
