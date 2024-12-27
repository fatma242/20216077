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
                        // If on a Unix-like OS (Linux/macOS), use sh to execute the script
                        sh './script.sh'
                    } else {
                        // If on Windows, use Git Bash to run the script
                        bat 'bash script.sh'
                    }
                }
            }
        }
    }
}
