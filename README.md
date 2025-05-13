Explanation of Files
- `main.bicep` – The entry point that calls various modules (networking.bicep, compute.bicep, etc.).
- `modules/` – Folder containing reusable components, such as networking, compute resources, and storage.
- `environments/` – Stores parameter files for different environments (e.g., `dev.parameters.json` for development, `prod.parameters.json` for production).
- `deploy.sh` – A script to automate deployment using Azure CLI.
- `README.md` – Documentation on how to deploy and manage the project.

Usage:
```bash
./deploy.sh <dev|qa|prod>
```
This will deploy the infrastructure to the specified environment using the corresponding parameter file.
Logs will be saved to deploy-<environment>.log.