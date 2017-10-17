pipeline {
    agent any

    stages {
        stage('Terraform Plan Approval') {
            steps {
            stage('Clone sources') {
                git url: 'https://github.com/jfrogdev/project-examples.git'
                sh 'Terraform plan'

                echo "Getting Terraform plan output..."
                echo "Raising Jira ticket for deployment approval..."
                input "Deploy to staging?"
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