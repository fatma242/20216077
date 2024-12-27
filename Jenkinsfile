pipeline {
    agent any // Runs on any available agent
    stages {
        stage('Clone Repository') { 
            steps {
                git(url: 'https://github.com/fatma242/20216077', branch: 'main')
            }
        }
        stage('Execute Script') { 
            steps {
                sh './script.sh' 
            }
        }
    }
}
