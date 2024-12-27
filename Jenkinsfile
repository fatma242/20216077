pipeline {
    agent any // Runs on any available agent
    stages {
        stage('Clone Repository') { 
            steps {
                git branch: 'main', url: https://github.com/fatma242/20216077
            }
        }
        stage('Execute Script') { 
            steps {
                sh './script.sh' 
            }
        }
    }
}
