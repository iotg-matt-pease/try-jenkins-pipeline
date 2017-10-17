pipeline {
    agent any

    stages {
        stage('Terraform Plan Approval') {
            steps {
                echo "Running Terraform plan..."
                echo "Getting Terraform plan output..."
                echo "Raising Jira ticket for deployment approval..."
            }
        }
        stage('Staging') {
            steps {
                echo "Running Terraform..."
                echo "Setting up config..."
                echo "Setting up SSH config..."
                echo "Running Ansible to provision and deploy applications..."
            }
        }
    }
}