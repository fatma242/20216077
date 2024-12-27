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
                script {
                    if (isUnix()) {
                        sh './script.sh'
                    } else {
                        bat '"C:\\Program Files\\Git\\bin\\bash.exe" script.sh'
                    }
                }
            }
        }
    }
}
