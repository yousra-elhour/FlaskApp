# Flask DevOps Project

A Flask web application with CI/CD pipeline using GitHub Actions.

## Features

- Flask web application with multiple routes (Home, Contact, About)
- Bootstrap frontend framework
- Automated testing with pytest
- CI/CD pipeline with GitHub Actions
- Ready for Azure deployment

## Setup

### Prerequisites

- Python 3.9+
- Azure account
- Azure CLI
- Terraform

### Local Development

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
```

2. Create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the application:

```bash
python -m flask run
```

5. Run tests:

```bash
pytest tests/
```

## CI/CD Pipeline

The GitHub Actions workflow (`.github/workflows/devops-app.yml`) automatically:

- Sets up Python 3.9
- Installs dependencies
- Runs tests
- Deploys to Azure (when configured)

## Azure Deployment

This project is configured for deployment to Azure App Service using Terraform and Azure CLI.

## Project Structure

```
FlaskWebProject1/
├── .github/workflows/          # GitHub Actions workflows
├── static/                     # Static files (CSS, JS, fonts)
├── templates/                  # HTML templates
├── tests/                      # Test files
├── __init__.py                # Flask app initialization
├── views.py                   # Route definitions
├── requirements.txt           # Python dependencies
└── README.md                  # This file
```
