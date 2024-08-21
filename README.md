# Dealer Review Application

## Overview

This project is a dealer review application built using Django. The app allows users to view a list of car dealers, view details of specific dealers, and add reviews for them. The application interacts with cloud functions to retrieve and display dealer information.

## Features

- **Static Pages**: Initial setup of several static pages for the application.
- **User Management**: Added templates and views for user registration, login, and management.
- **Dealer List & Details**: Created views and templates to list dealers and show detailed information about each dealer.
- **Review Submission**: Integrated functionality for users to add reviews for dealers.
- **Proxy Services**: Developed proxy services to call cloud functions, convert JSON responses to Python objects, and return them as HTTP responses.

## Development

### Initial Setup

1. **Repository Preparation**: The repository was prepared, and an app skeleton was cloned.
2. **Static Pages**: Several static pages were created and tested.
3. **User Management**: Added user management-related templates and views.

### Core Features

1. **Dealer List & Details**: Implemented dealer list and detailed views, along with a provision for adding reviews.
2. **Proxy Services**: Developed services to call cloud functions and handle responses.

### Linting and Code Quality

- **GitHub Actions**: Linting has been added to the repository to automatically check for coding style errors and syntax issues whenever a pull request is created or a branch is merged into the main branch.

## Deployment

To deploy the application, use the following command with your deployment file:

```bash
kubectl apply -f deployment.yaml
```

To see the running application, use port-forwarding:

```bash
kubectl port-forward deployment.apps/dealership 8000:8000
```

### Access the Application

1. Click the "Dealership Application" button or use the "Skills Network Toolbox."
2. Enter port `8000` and launch to access the application.
3. You can log in, view dealers, review them, and log out.

### Deployment URL

You can also access the application through the following link:

[Dealer Review Application](https://mathiaspelle-8000.theianext-0-labs-prod-misc-tools-us-east-0.proxy.cognitiveclass.ai/)

## Future Work

- **Car Make Models**: The next phase will involve creating car/make-related models, templates, and views.
- **Team Collaboration**: The team is expanding, and measures are being put in place to ensure smooth collaboration, such as enforcing code quality checks and style guides.
