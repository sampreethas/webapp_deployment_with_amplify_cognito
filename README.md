# React App Deployment with AWS Amplify

This project is a **React application** deployed using **AWS Amplify**. Below are the steps followed to set up, configure, and deploy the application.

## Prerequisites
Ensure you have the following installed before proceeding:
- **Node.js & npm** (https://nodejs.org/)
- **AWS CLI** (https://aws.amazon.com/cli/)
- **Amplify CLI** (https://docs.amplify.aws/cli/start/install/)
- **Git** (https://git-scm.com/)
- A GitHub repository for version control

## Installation & Setup

### 1. Install AWS Amplify CLI
```sh
npm install -g @aws-amplify/cli
```

### 2. Configure AWS Amplify
```sh
amplify configure
```
Follow the prompts to set up an AWS IAM user and configure credentials.

### 3. Create a New React App
```sh
npx create-react-app <name-of-your-app>
cd <name-of-your-app>
```

### 4. Initialize AWS Amplify
```sh
amplify init
```
Follow the on-screen prompts to set up Amplify for your project.

### 5. Add Authentication (AWS Cognito)
```sh
amplify add auth
```
Select the default configuration or customize as needed.

### 6. Deploy Amplify Resources
```sh
amplify push
```
This deploys the authentication and other Amplify services to AWS. You can view the app directly from AWS Amplify deployment section via a link.
Any changes in repo will trigger CI/CD automatically with AWS Amplify.

`Example of a deployed app`

![image](https://github.com/user-attachments/assets/ace16316-6261-4b50-a56b-cc3cb3974708)

The deployment also contains link to github code, commit history and logs for detail analysis.

![image](https://github.com/user-attachments/assets/1460ad9d-efc0-4b25-8efe-629808b3b55b)


### 7. Install AWS Amplify Libraries
```sh
npm install aws-amplify @aws-amplify/ui-react
```

### 8. Start the React App from terminal
```sh
npm start
```
This launches the application in development mode.

## Version Control 

### 9. Initialize Git Repository
```sh
git init
git add .
git commit -m "Initial commit"
```

### 10. Set Up Git Branch
```sh
git branch -M main
```

### 11. Connect to Remote Repository
```sh
git remote add origin <repository-URL>
```

### 12. Push Code to GitHub
```sh
git push -u origin main
```

## Next Steps
- Add additional AWS Amplify services like API, storage, or hosting as needed.
- Customize authentication flows using AWS Cognito.

## References
- [AWS Amplify Docs](https://docs.amplify.aws/)
- [React Documentation](https://reactjs.org/)
- [GitHub Docs](https://docs.github.com/)


