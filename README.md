# Amplify React Deployment

This project demonstrates deploying a React application to AWS using a GitHub-connected CI/CD workflow with AWS Amplify.

## Architecture Diagram
![Amplify React Deployment](diagrams/amplify-react-deployment.png)

## Overview
A React application is developed locally, pushed to GitHub, and automatically built and deployed by AWS Amplify. Each push to the main branch triggers a new deployment and updates the public web application URL.

## Architecture Flow
1. The React application is developed locally using React + Vite.
2. Changes are committed and pushed to the GitHub repository (main branch).
3. AWS Amplify is connected to the GitHub repository.
4. Amplify automatically:
   - Pulls the latest code
   - Builds the React application
   - Deploys it to managed hosting
5. The application is served via a public HTTPS URL.

## Services Used
- GitHub (source control)
- AWS Amplify (CI/CD, build, and hosting)
- React + Vite (frontend application)

## Key Benefits
- Automatic deployments on every commit
- HTTPS-enabled public URL
- No server management
- Simple CI/CD workflow for frontend applications

## Result
A fully managed, continuously deployed React web application hosted on AWS.
