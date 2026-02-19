Azure-Powered Intelligent Task Management System
Overview
This project is a cloud-based task management system built with Microsoft technologies. It leverages Azure Cognitive Services, Azure Bot Service, and Azure Machine Learning to provide intelligent task recommendations, automated reminders, and advanced analytics. The system is fully integrated with Microsoft Teams and Office 365.

Features
Task Creation and Management
Intelligent Task Recommendations
Automated Reminders
Advanced Analytics Dashboard
Technologies Used
Front-End: React.js, TypeScript
Back-End: ASP.NET Core, C#
Cloud Services: Azure Functions, Azure Machine Learning, Azure Bot Service
CI/CD: Azure DevOps
Security: Azure Active Directory, Azure Key Vault
Getting Started
Prerequisites
Node.js and npm
.NET Core SDK
Azure Subscription
Installation
Clone the repository:

git clone https://github.com/yourusername/azure-task-management-system.git
Install the front-end dependencies:

cd frontend
npm install
Build and run the backend API:

cd backend
dotnet run
Deploy Azure Functions and Bot Service:

Follow the Azure documentation to deploy Functions and Bot Service.
Deployment
Use the provided Azure Pipelines YAML file to set up continuous integration and continuous deployment.
Contributing
Feel free to fork this project and submit pull requests. Contributions are welcome!

License
This project is licensed under the MIT License - see the LICENSE file for details.

✅ Verified Quickstart
The following commands were used to validate the repo structure and build the frontend bundle. The backend requires the .NET 6 SDK to run locally.

cd frontend
npm run build
To run the backend API after installing the .NET 6 SDK:

./scripts/run_backend.sh
To run the frontend dev server:

./scripts/run_frontend.sh
To run the automated smoke test (requires .NET 6 SDK and curl):

./scripts/smoke_test.sh
Troubleshooting
dotnet: command not found: Install the .NET 6 SDK and ensure dotnet is on your PATH.
Backend not responding on http://localhost:5055: The smoke test starts the API on port 5055; ensure the port is free.
Missing node_modules: Run npm install in the frontend directory or use ./scripts/run_frontend.sh which installs dependencies automatically if needed.
