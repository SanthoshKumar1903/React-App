### 🚀 CI/CD with GitHub Actions and PM2

This project includes a full CI/CD pipeline with GitHub Actions:

- **CI Workflow (`test.yml`)**
  - Installs Node and dependencies
  - Starts the dev server with `pm2`
  - Runs tests
  - Cleans up all PM2 processes

- **CD Workflow (`deploy.yml`)**
  - Builds the React app
  - Simulates a production server using `pm2` + `serve`
  - Deploys the build to GitHub Pages
  - All processes are managed and terminated using `pm2`
