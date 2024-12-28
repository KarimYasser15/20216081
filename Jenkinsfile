pipeline {
    agent any
    stages {
        stage('Pull Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/KarimYasser15/20216081'
            }
        }
        stage('Execute Script') {
            steps {
                script {
                    if (isUnix()) {
                        sh './run_ls.sh' // For Linux/Unix
                    } else {
                        bat 'run_ls.bat' // For Windows
                    }
                }
            }
        }
    }
}
