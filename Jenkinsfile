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
                bat 'run_ls.bat'
            }
        }
    }
}
