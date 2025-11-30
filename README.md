# React Azure App

This is a minimal Vite + React app preconfigured for deployment to Azure Static Web Apps.

Local development

1. Install dependencies:

```powershell
cd react-azure-app
npm ci
npm run dev
```

2. Build for production:

```powershell
npm run build
```

Deploy to Azure (GitHub Actions / Azure Static Web Apps)

1. Create a Static Web App in the Azure Portal or via the `az` CLI.
2. In your GitHub repo, add a secret named `AZURE_STATIC_WEB_APPS_API_TOKEN` containing the deployment token from the Static Web App resource (Deployment Center).
3. Push this repo to GitHub on the `main` branch. The included GitHub Actions workflow will build and deploy automatically.

Alternative: use the Azure Portal "Deployment Center" to connect your repository directly.
