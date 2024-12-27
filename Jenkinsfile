pipeline {
    agent any
    tools {
        git 'Default' // Matches the name set in Git installations
    }
    stages {
        stage('Clone Repository') { 
            steps {
                git url: 'https://github.com/fatma242/20216077', branch: 'main'
            }
        }
        stage('Execute Script') { 
            steps {
                sh './script.sh'
            }
        }
    }
}
